# Kasada's p.js Deobfuscated

They obfuscated the script by replacing most strings with a function to grab the string from an array and decode it.

Ex:
`_0x36f133(0x5ee,'m6n4')`

0x5ee is the index and "m6n4" is a value used to decode the string from the array.

The array is not properly in order at first and it is rearranged when the script is first executed.

Note: Identifiers were replaced with more eye friendly ones
```js
;(function (juquana, jernae) {
    var gali = KPSDK_0x1a3a; // KPSDK_0x1a3a is the function that pulls from the array
    while (true) {
      try {
        var tuyetnhung = -parseInt(gali(1246, "ZrqT")) * parseInt(gali(1123, "SF8Y")) + parseInt(gali(866, "B&jL")) + parseInt(gali(488, "i&SL")) * parseInt(gali(749, "SF8Y")) + parseInt(gali(1404, "0mUP")) * parseInt(gali(1382, "VR1C")) + parseInt(gali(1566, "8%Ma")) * -parseInt(gali(937, "s$M0")) + parseInt(gali(1517, "KuSv")) * parseInt(gali(1258, "HY&U")) + -parseInt(gali(403, "s$M0")) * parseInt(gali(1201, "#jW1"));
        if (tuyetnhung === jernae) break; else juquana.push(juquana.shift());
      } catch (oshanna) {
        juquana.push(juquana.shift());
      }
    }
  }(KPSDK_0xf49f, 464424) // KPSDK_0xf49f is the array of encoded strings
```

