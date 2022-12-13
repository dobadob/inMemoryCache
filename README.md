This is my homework for the first section of the Golang Ninja course.

The package implements in-memory cache ability.

There are examples of usage below:

	func main() {
    
        myCache := cache.New()
    
        myCache.Set("userId", 42)
	    userId := myCache.Get("userId")

	    fmt.Println(userId)		//42

	    myCache.Delete("userId")
	    userId := myCache.Get("userId")

	    fmt.Println(userId)		//nil
    }
