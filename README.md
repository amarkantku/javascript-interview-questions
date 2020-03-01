# javascript-interview-questions
Frequently asked top javascript interview questions.


1. Write a custom indexOf() array function.

Array.prototype.itemIndexOf = function(searchElement, fromIndex = undefined) {
  var searchIndex = fromIndex || 0;
  for (var index = searchIndex, len = this.length; index < len; index++) {
    if (this[index] === searchElement) {
      return index;
    }
  }
  return -1;
}

console.log([1, 2, 3, 4, 5].itemIndexOf(5, 5));


