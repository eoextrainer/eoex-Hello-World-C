


# Hello World ! ( C )

Hi! This is **EOEX**, and I present to you the "Hello World (C)" project. 
This project aims to practice the time tested tradition of displaying the **"Hello World"** message on a computer screen; this time using the **C programming language**. If you want to learn about EOEX and our projects, following our adventures here and on our social media. 
We hope that you will enjoy this educational journey ;-)

## 1- Situation
  **Customer Benefits:**
        to display the message "Hello World" on the computer screen
    
   **User Story:**
 - **As a** computer user
 - **I want** to display the message "Hello World" on the computer screen
 - **So that** I can I can practice this time tested tradition

**Acceptance Criteria:**
 - [ ] the source code must be written in the C programming language
 - [ ] the source code must be compiled using a script
 - [ ] the unit test must test each method of this program 
 - [ ] the soure code must be deployed to a version control system

    
## 2- Problem Set 

> Create a computer program that displays the message "Hello World" on the computer screen (the standard output)

## 3- Design

 1. program greetings
 2. data inputs
 3. data validations
 4. data processing & boundary conditions
 5. error and exception handling
 6. data output
 7. program farewell/exit

## 4- Architecture
- import the stdio.h C library
- declare the main() function | The argc and argvar parameters allow command-line arguments,

## 5- Implementation

	#include <stdio.h>
	#include <CUnit/CUnit.h>        // unit testing framework
	
	int main(int argc, char * argvar[])
	{
		// Data Daclarations
		char greetings[] = "Hello World";
		
		// Data inputs 

		// Data validations

		// Data processing & boundary conditions

		// Error & exception handling

		// Data output
		printf("%s", greetings);
		
		// Program farewell/exit
		return 0;
	}


## 6- Testing
    // In C, this means testing functions and modules to verify that they return correct outputs for given inputs. Unit tests help catch bugs early, reduce regression issues, and improve code quality.
    
    # On Ubuntu 24.04.03 LTS
    - install CUnit: sudo apt-get install libcunit1 libcunit1-doc libcunit1-dev
    - inside the source code include: #include <CUnit/CUnit.h>
        Write functions for tests (and suite init/cleanup if necessary).
        Initialize the test registry - CU_initialize_registry()
        Add suites to the test registry - CU_add_suite()
        Add tests to the suites - CU_add_test()
        Run tests using an appropriate interface, e.g. CU_console_run_tests
        Cleanup the test registry - CU_cleanup_registry
    
    testing functions
    testing modules
1. setup
2. act 
3. assert
    

## 7- Packaging
    compilation: 
    

	gcc -o hello-world-c hello-world-c.c -lcunit
    echo "gcc -o hello-world-c hello-world-c.c -lcunit" >> script_hello-world-c.sh
    chmod -v +x script_hello-world-c.sh
        
    compilation script:
    #!/usr/bin/bash

    # setup script variables
    sourceFile="hello-world-c"
    sourceCode=$sourceFile".c"
    log_out=$sourceFile".out"
    log_error=$sourceFile"_error.out"

    # Variable Validations
    echo "Source File: " $sourceFile
    echo "Source Code: " $sourceCode
    echo "Output File: " $log_out
    echo "Error File: " $log_error

    function compile_code()
    {
	    echo "Compiling code: " $sourceCode
	    gcc -v -o $sourceFile $sourceCode -lcunit > $log_out 2>&1 $log_error
    }

    function run_code()
    {
	    echo "Running code: " $sourceFile
    }

    # Main Script Code
    compile_code
    run_code


## 8- Deployment

## 9- Delivery & Execution
<img width="640" height="556" alt="hello-world-c" src="https://github.com/user-attachments/assets/d86033a8-55f1-424c-86de-818d49ee3325" />


## 10- Documentation & Presentation
