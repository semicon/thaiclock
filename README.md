# Thai clock

![image](https://user-images.githubusercontent.com/30399464/152095700-bdc8edde-7420-4f02-9754-e737d5f842f0.png)

# เปลี่ยนเลขอารบิคเป็นเลขไทย

      function thaiNumber(numb){
         var array = {"1":"๑", "2":"๒", "3":"๓", "4" : "๔", "5" : "๕", "6" : "๖", "7" : "๗", "8" : "๘", "9" : "๙", "0" : "๐"};
         var str = numb.toString();
         for (var val in array) {
            str = str.split(val).join(array[val]);
          }
         return str;
      }
      
# เดือนภาษาไทย

      function thaiMonth() {
        var date = new Date();
        var DATE = date.getDate();
        var MONTH = ["มกราคม","กุมภาพันธ์","มีนาคม","เมษายน","พฤษภาคม","มิถุนายน","กรกฎาคม","สิงหาคม","กันยายน","ตุลาคม","พฤศจิกายน","ธันวาคม"];
        var THAI_MONTH = MONTH[date.getMonth()];

        return THAI_MONTH
      }
