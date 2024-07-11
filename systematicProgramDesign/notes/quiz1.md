
Problem:
Design a function that consumes two images and produces true if the first is larger than the second.

;; Image, Image -> Boolen: **Signature**

;; Takes as argument two images and returns true if the area of the first is bigger than the second one. **Purpose**

(check-expect (larger_image? (img1 img2)) False))
(check-expect (larger_image? (img3 img2)) True))
(check-expect (larger_image? (img1 img4)) False))

; (define (larger_image? img1 img2) true)  **Stub**

 ;(define (larger_img? img1 img2) **Template**
    (...img1 img2))

(define (large_image? first_img.area second_img.area)
        (> (* first_img.height first_img.width) (* first_img.height first_img.width)))


