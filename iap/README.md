go-iap
======

A go implementation for verifying In App Purchases via apple.

### Usage

``` 
package main

import (
	"fmt"
	"github.com/antigloss/go/iap"
	"log"
)

func main() {
	receipt, err := goiap.VerifyReceipt("receipt",true) // Uses the sandbox environment

	if err != nil {
	  log.Fatal(err)
	}
	
	fmt.Println("Got receipt", receipt)
}
```