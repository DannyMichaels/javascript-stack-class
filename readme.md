class Stack {
    // Array is used to implement stack
    constructor() {
        this.items = [];
		}
  
    // Functions to be implemented
    push(item) {
			this.items.push(item)
		}
	
    pop() {
		// return top most element in the stack
    // and removes it from the stack
    // Underflow if stack is empty
    if (this.items.length === 0)  return "Underflow";
    return this.items.pop();
		}
	
    peek() {
			  return this.items[this.items.length - 1];
		}
	
    isEmpty() {
		  return this.items.length === 0;
		}
	
    printStack() {
	  	let str = "";
    	for (let i = 0; i < this.items.length; i++) {
        str += this.items[i] + " ";
			}
   			return str;
		}
}
