
# problem1

Design a function that consumes an image and determines whether the image is tall.


## Solution

First of all, what is considered tall? I need to compared against something to know that. 

Image -> Boolean (is tall or not) **Signarture**

If the image height is bigger than its width, produces true. Otherwise returns false. **(When designing a function which produces a boolean, the purpose specifies how to interpret the output)**


(define (isTall image) false)

check-expect (isTall (img)) True)
check-expect (isTall (img)) False)


(define (isTall img)
    (if
    (>= (img.height) (img.width))
    False
    (< (img.height) (img.width))
    True)
