---
title: "day_01"
author: "Muhammad Zain Zameer"
date: "2024-07-04"
output: html_document
---

# Introduction to R

Following are the basics commands and operations in R language:

-   Calculations

    We can perform basic calculations in our text editor like below:

    -   25 **/** 2
    -   25 **\*** 5
    -   45 **+** 6
    -   7 **-** 2

-   Comments

    Comments are the best way to make someone fully understand, what the code is about. Starts from '**\# [Your Text]**'

    ``` r
    # Hello, I am comment which makes it easier for everyone to understand the logic
    ```

-   Data Types

    Following are the data types in R language:

    -   **Numeric**: It refers to data that consists of numbers, which can be either integers or floating-point numbers. This data type is used to perform arithmetic operations and mathematical computations. Numeric values in R can be positive, negative, or zero and can include decimal points.

    ``` r
    x <- 42    # Integer numeric value
    y <- 3.14  # Floating-point numeric value
    ```

    -   **Character**: It refers to data that consists of strings or sequences of characters. Character values are used to represent text and are enclosed in either single or double quotes.

    ``` r
    name <- "John Doe"         # Character value with double quotes
    greeting <- 'Hello, World' # Character value with single quotes
    ```

    -   **Logical**: The logical data type represents boolean values, which can be either TRUE or FALSE. Logical values are used for conditional statements, comparisons, and control flow in programming.

    ``` r
    is_true <- TRUE   # Logical value TRUE
    is_false <- FALSE # Logical value FALSE
    ```

    -   **Vectors**: It is a basic data structure that contains elements of the same type. Vectors are used to store a sequence of data elements and can be numeric, character, logical, or any other type. They are created using the c() function.

    ``` r
    numeric_vector <- c(1, 2, 3, 4, 5)          # Numeric vector
    character_vector <- c("apple", "peach")    # Character vector
    logical_vector <- c(TRUE, FALSE, TRUE)      # Logical vector
    ```

-   Class Method:

    class(element) will return you the the class name of which type of data is this.

    ``` r
    x <- 42    
    class(x)  # Output: class <numeric>
    ```

-   Variables:

    Variables are the containers in which you store your data and that data can be of any type.It can't start from any number or special character, but it can end with a digit.

    ``` r
    name <- "John Doe"         # String value 
    lucky_No <- 272.2          # floating point value
    age <- 20                  # integer value
    letter <- 'Z'              # character value 
    check <- TRUE              # boolean/logical value
    vec1 <- c(1,2,3,4)         # vector data 
    ```

    We can create variables of data type by using assignment operator.

-   Vectors:

    In R, a vector is a basic data structure that stores elements of the same type. Vectors can be numeric, character, logical, or any other type, and they are created using the `c()` function. Vectors are essential for data manipulation and analysis, allowing efficient storage and operations on sequences of data elements.

    ``` r
    # Numeric vector
    numeric_vector <- c(1, 2, 3, 4, 5)

    # Character vector
    character_vector <- c("apple", "banana", "cherry")

    # Logical vector
    logical_vector <- c(TRUE, FALSE, TRUE)
    ```

    Following are some built in functions you can use for vector:

    ``` r
    # Numeric vector
    numeric_vector <- c(1, 2, 3, 4, 5)

    # Checking the type of a vector
    typeof(numeric_vector)

    # Checking the length of a vector
    length(numeric_vector)

    # Getting the values by indexing in vector
    numeric_vector[1]
    ```

    **Note**: Indexing start from 1 in R language.

-   Conditionals:

    In R, conditionals are used to execute different blocks of code based on certain conditions. The primary conditional statements in R are `if`, `else if`, and `else`. Here's how each of them works:

    -   **if Statement**:

        The `if` statement allows you to execute a block of code only if a specified condition is true.

    ``` r
    x <- 10

    if (x > 5) {
      print("x is greater than 5")
    }
    ```

    -   **else if Statement**:

        The `else if` statement allows you to test multiple conditions. If the first condition is false, the `else if` statement is evaluated.

    ``` r
    x <- 10

    if (x > 10) {
      print("x is greater than 10")
    } else if (x == 10) {
      print("x is equal to 10")
    }
    ```

    -   **else Statement**:

        The `else` statement allows you to execute a block of code if none of the previous conditions are true.

    ``` r
    x <- 10

    if (x > 10) {
      print("x is greater than 10")
    } else if (x == 10) {
      print("x is equal to 10")
    } else {
      print("x is less than 10")
    }
    ```

    -   **Nested if Statements**:

        You can also nest `if` statements within each other.

    ``` r
    x <- 10
    y <- 5

    if (x > 5) {
      if (y > 5) {
        print("Both x and y are greater than 5")
      } else {
        print("x is greater than 5 but y is not")
      }
    }
    ```

    -   **Vectorized if else**:

        For vector operations, you can use `ifelse`, which is a vectorized version of `if-else`

    ``` r
    x <- c(10, 4, 6)

    result <- ifelse(x > 5, "Greater than 5", "Not greater than 5")
    print(result)
    ```

-   Logical Operators:

    Logical operators in R are used to perform logical operations on values. These operators return Boolean values (`TRUE` or `FALSE`). Here are the main logical operators in R:

    -   **`&` (Element-wise AND)**:

        The `&` operator returns `TRUE` if both operands are `TRUE`. It operates element-wise on vectors.

        ``` r
        a <- c(TRUE, FALSE, TRUE)
        b <- c(TRUE, TRUE, FALSE)
        result <- a & b
        print(result)  # [1]  TRUE FALSE FALSE
        ```

    -   **\| (Element-wise OR)**:

        The \| operator returns TRUE if at least one of the operands is TRUE. It operates element-wise on vectors.

        ``` r
        a <- c(TRUE, FALSE, TRUE)
        b <- c(TRUE, TRUE, FALSE)
        result <- a | b
        print(result)  # [1] TRUE TRUE TRUE
        ```

    -   **! (NOT)**:

        The `!` operator returns `TRUE` if the operand is `FALSE` and vice versa. It negates the Boolean value.

        ``` r
        a <- TRUE
        result <- !a
        print(result)  # [1] FALSE
        ```

    -   **Example Usage in Conditional Statements**:

        You can combine logical operators with conditional statements for more complex logic.

        ``` r
        x <- 5
        y <- 10

        if (x < 10 & y > 5) {
          print("Both conditions are TRUE")
        }

        if (x < 10 | y > 15) {
          print("At least one condition is TRUE")
        }

        if (!x == 10) {
          print("x is not equal to 10")
        }
        ```

-   Some useful built-in functions:

    -   **sqrt()**:

        Calculates the square root of a number or each element in a vector.

        ``` r
        # Square root of a single number
        result <- sqrt(16)
        print(result)  # [1] 4

        # Square root of each element in a vector
        numbers <- c(4, 9, 16, 25)
        result <- sqrt(numbers)
        print(result)  # [1] 2 3 4 5
        ```

    -   **sort()**:

        Sorts the elements of a vector in ascending or descending order.

        ``` r
        # Sorting in ascending order (default)
        numbers <- c(5, 3, 8, 1)
        result <- sort(numbers)
        print(result)  # [1] 1 3 5 8

        # Sorting in descending order
        result <- sort(numbers, decreasing = TRUE)
        print(result)  # [1] 8 5 3 1
        ```

    -   **length()**:

        Returns the number of elements in a vector or the length of an object.

        ``` r
        # Length of a vector
        numbers <- c(5, 3, 8, 1)
        result <- length(numbers)
        print(result)  # [1] 4

        # Length of a character string
        text <- "Hello, world!"
        result <- length(text)
        print(result)  # [1] 1
        ```

    -   **sum()**:

        Calculates the sum of the elements in a vector.

        ``` r
        # Sum of elements in a numeric vector
        numbers <- c(5, 3, 8, 1)
        result <- sum(numbers)
        print(result)  # [1] 17

        # Sum of elements in a logical vector (TRUE = 1, FALSE = 0)
        logical_vector <- c(TRUE, FALSE, TRUE, TRUE)
        result <- sum(logical_vector)
        print(result)  # [1] 3
        ```

    -   **unique()**:

        Extracts the unique elements from a vector.

        ``` r
        # Unique elements in a numeric vector
        numbers <- c(5, 3, 8, 1, 3, 5, 8)
        result <- unique(numbers)
        print(result)  # [1] 5 3 8 1

        # Unique elements in a character vector
        text <- c("apple", "banana", "apple", "orange")
        result <- unique(text)
        print(result)  # [1] "apple"  "banana" "orange"
        ```

    -   **floor()**:

        Rounds down each element in a vector to the nearest integer.

        ``` r
        # Floor function example
        numbers <- c(1.5, 2.3, 3.7, 4.9)
        result <- floor(numbers)
        print(result)  # [1] 1 2 3 4
        ```

    -   **ceiling()**:

        Rounds up each element in a vector to the nearest integer.

        ``` r
        # Ceiling function example
        numbers <- c(1.5, 2.3, 3.7, 4.9)
        result <- ceiling(numbers)
        print(result)  # [1] 2 3 4 5
        ```
