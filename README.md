# TrimmedMean

## Description
In this project we create a function for calculating the trimmedmean using go language package to get the accurate results using minimum memory and resources with minimum time. The main.go file contains the example implementation of the program or function and the trimmedmeancalc.R contains the verification of the results using R language built in functions.
## Dependencies
- Go Language download from go.dev/doc/install
- [trimmedmean](https://github.com/dani67894/TrimmedMean) - A Go package for computing trimmed mean.
- (in case you have to verify the results) R language download from https://cran.r-project.org/bin/windows/base/ 

## Installation
To properly use the TrimmedMean package in your project, follow these steps:
-Clone the Repository: First, clone the repository to your local machine.
-Initialize Your Project: Set up your Go project in a different directory.
-Use the Package: Import and use the TrimmedMean package in your Go project.

Step 1: Clone the Repository
Open PowerShell and run the following command to clone the repository:
git clone https://github.com/dani67894/TrimmedMean.git

Step 2: Initialize Your Project
Navigate to a directory where you want to create your Go project and initialize a new module:
mkdir MyGoProject
cd MyGoProject

Step 3: Use the Package
In your new Go project directory, create a Go file (e.g., main.go) and import the TrimmedMean package as the following example or the example given in main.go file of repository :
package main
import (
	"fmt"
	"github.com/dani67894/TrimmedMean/trimmedmean"
)
func main() {
	data := []float64{1.0, 2.0, 3.0, 4.0, 5.0} 
	trimmedMean, err := trimmedmean.TrimmedMean(data, 0.1)
	if err != nil {
		fmt.Println("Error computing trimmed mean:", err)
		return
	}
	fmt.Println("Trimmed Mean:", trimmedMean)
}

Step 4: Run Your Program
Finally, run your Go program:
go run main.go

##Example usage
As provided the example in the main.go file. 
