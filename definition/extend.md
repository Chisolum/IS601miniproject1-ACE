# Extend Class

The extends keyword is used in class declarations or class expressions to create a class which is a child of another class. Also, the extends keyword can be used to subclass custom classes as well as built-in objects. The .prototype of the extension must be an Object or null. Below is an example from developer.mozilla.org.
You can inherit attributes and methods from one class to another by grouping the "inheritance concept" into two categories:
•	subclass (child) - the class that inherits from another class
•	superclass (parent) - the class being inherited from
To inherit from a class, use the extends keyword.
class formatDate extends Date {
  constructor(dateStr) {
    super(dateStr);
  }

  getFormattedDate() {
    var months = ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun',
                  'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec'];

    return `${this.getDate()}-${months[this.getMonth()]}-${this.getFullYear()}`;
  }
}

console.log(new formatDate('August 19, 1975 23:15:30').getFormattedDate());
// expected output: "19-Aug-1975"


