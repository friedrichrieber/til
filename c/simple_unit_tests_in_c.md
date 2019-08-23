# Simple Unit Tests in C with Check

My solution for simple unit tests in the c language is a library called [check](https://libcheck.github.io/check/doc/check_html/check_3.html#Test-a-Little). And with a little parsing tool called ```checkmk``` you can create test in a simple and fast way. 

# Usage

I used the Tutorial from this [stackoverflow post](https://stackoverflow.com/questions/14176180/is-there-a-more-basic-tutorial-for-the-c-unit-testing-framework-check).

And for check to work you need to include these librarys when compiling

```-lcheck_pic -lrt -lm -lsubunit -pthread```

which i got from this [stackoverflow post](https://stackoverflow.com/questions/39573980/libcheck-test-fails-to-link).

## Sources 

https://libcheck.github.io/check/doc/check_html/check_3.html#Test-a-Little
https://stackoverflow.com/questions/14176180/is-there-a-more-basic-tutorial-for-the-c-unit-testing-framework-check
https://stackoverflow.com/questions/39573980/libcheck-test-fails-to-link
