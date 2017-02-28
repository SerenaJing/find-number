 The findNum is a function to search for the number
 
    function findNum (arr, num) {
      var length = arr.length;
      var temp = 0;
      if(arr[length-1]>num) {
        temp = length-2;
        while(arr[temp] != num && arr[temp]<num) {
          temp--;
        }
      } else {
        while(arr[temp] != num && arr[temp]<arr[temp+1]) {
          temp++;
        }
      }
      if(arr[temp] == num) {
        return true;
      }
      return false;
    }
    
This is a test, you can change the arr and num for any test.

If the num in the arr, the function will return true, other return false.

    var arr = [7,8,9,1,2,3,4,5,6];
    var num = 10;
    var result = findNum (arr, num);
    alert(result);
