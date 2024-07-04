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
