# Context-this-

var person = {
 name: 'John Doe',
 age: 42,
 gender: 'male',
 bio: function() {
 console.log('My name is ' + this.name);
 }
};
person.bio(); // logs "My name is John Doe"
var bio = person.bio;
bio(); // logs "My name is undefined"
