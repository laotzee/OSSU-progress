
# Design of Data

- When we design data, we make decisions about all the functions that later operate on that data.

- Data definitions explain how information is represented as data. It describes:
    - How to form data of a new type
    - How to represent information as data
    - How to interpret data as information
    - Template for operating on data.
Data definition also simplifies functions:
    - restricts data consumed
    - restricts data produced
    - Helps generate examples
    - Provides a template

- The problem that data designing solves: 
- Problem Domain
- ' Identifying the structure of the information is a key step in program design'
- 'As data definitions get more sophisticated, you will see that choosing the structure ot use is a point of leverage in designing the overall program'
- 'Once we identify the structure of the information, that give us the
    structure of the data used to represent it, which gives us the structure of
    the template, which gives us the structure of the function, and also we get
    guidance about the test for that function'
- **Identifying the structure of the information is a key step in program design**
- :


## Exercise 1

;; seat is Integer[1,32]
;; interp. number of the seat in a row

(define  seat1 32) ; aisle
(define  seat2 1)  ; aisle
(define  seat3 16) ; middle


# exercise 1
( define (fn-for-seat seat1)
    ...seat1)

;; Template rules used:
;; - atomic non-distinctic: seat[0, 32]


# exercise 2 (enumeration)

;; studentGrade is one of:
;; - 'A'    5
;; - 'B'    4
;; - 'C'    3
;; - 'D'    2
;; - 'F'    1

;; Interp. letter grade in a course
;; <examples are redundant for enumaerations>

(define (fn-for-studentGrade st)
    (cond [(string=? st 'A') (...)]
          [(string=? st 'B') (...)]
          [(string=? st 'C') (...)]
          [(string=? st 'D') (...)]
          [(string=? st 'F') (...)]))

;; Template rules used:
;; one of: 3 cases
;; atomic distinc value: "A"
;; atomic distinc value: "B"
;; atomic distinc value: "C"
;; atomic distinc value: "D"
;; atomic distinc value: "F"

# exercise 3 (Itemization)

;; state is one of:
;; - false
;; - Natural [1, 10]
;; - 'complete'

;; interp.
;; false means countdown  has not yet started
;; natural [1, 10] describes describes seconds before midnight
;; 'complete' menas count down is over

;; (define cd1 false)
;; (define cd2 10)
;; (define cd3 'complete')

(define (fn-for-state state) 
    (cond[(false? state) (...)]
         [(number? state) (...state))]
         [(string=? state 'complete' (...))]))

;; Template rules used:
;; one of: 3 cases
;; atomic distinct:: false
;; atomic non-distinct natural [1, 10]
;; atomic distinct: 'complete'

 
# Exercise 4 (HtDF with Inverval)

;; Data definitions:

;; seatNum is Natural[1, 32]
;; interp. Seat numbers in a row, 1 and 32 aisle seats

( define seat1 1 ); aisle
( define seat1 15 ); middle
( define seat1 32 ); aisle

(define (fn-for-seat st)
    (...st))


;; Template rules used:
;; attomic non-distinct: Natural[1,32]

;; isAisle? -> boolean ;signature
;; returns true is the given seat is on the aisle

; (define (isAisle?) false)

(check-expect (isAisle? st32) true)
(check-expect (isAisle? st14) false)
(check-expect (isAisle? st1) true)

(define (isAisle? st)
    (or (= 1 st)
        (= 32 st)))

# exercise 5 (HtDF with Enumeration)


;; letterGrade > letterGrade 
;; produce the next highest letter grade (no changes for A)


( define (nextGrade letterGrade) 'A')

(check-expect (nextGrade lg1) 'A') ;; being 'B' the grade
(check-expect (nextGrade lg1) 'B') ;; being 'C' the grade
(check-expect (nextGrade lg1) 'A') ;; being 'A' the grade


( define (nextGrade lg)
    (cond[(string? l  'A') ('A')]
         [(string? lg 'B') ('A')]
         [(string? lg 'C') ('B')]))

# exercise 6 (HtFD with Itemization)

;; CountDown > Image
;; produce image of the state of countdown

( define (ct-img ct) (square 0 'solid') )

(check-expect (ct-img 10))
(check-expect (ct-img 1))
(check-expect (ct-img 'complete'))
(check-expect (ct-img false))

( define (ct-img CountDown) 
    (cond[false? CountDown] ( square 0 'solid' 'white')
         [and (number? CountDown) (...CountDown)]
         [else ('Happy New Year!')]))
