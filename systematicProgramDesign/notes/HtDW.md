 

 #These are functions of big bang structure. 

 - on-tick
 - to-draw



# Exercise 1


## Domain Analysis

1.- Sketch Program Scenarios


2.- Identify Constant Information

- MTS
- Y cordinate
- Cow image
- Speed
- height
- width


3.- Identify Changing Information

- X coordinate
- Cow's direction
-


4.- Identify Big-bang options


- on-tick
- to-draw
- on-key




( define MTS x )
( define cow_img y )
( define speed z )

( define height 1200 )
( define width 700 )

( define cow_y (/ height 2) )


(define-struct cow_state (x, dx))

;; cow_state is (make-cow_state Number String)
;; interp. cow_state dictates the x coordinate of the image
;;         and dx the direction of the cow

(define (fn-for-cow cow_state)
    (...(cow_state-x b)     ;Number
        (cow_state-dx)))    ;String

;; Template rules used:
;;; - compound: 2 fields
