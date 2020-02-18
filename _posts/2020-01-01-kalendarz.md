---
layout: post
title: "Kalendarz"
date: 2020-01-01
---

Czy jest lepiej czy jest źlej?

<style>
.bad{background-color:red}
.uneasy{background-color:#ffaaaa}
.nice{background-color:green}
.quiteok{background-color:#aaffaa}
.uneasyandnice{background-image: linear-gradient(to bottom right, #ffaaaa 0%, #ffaaaa 50%, green 50%, green 100%);}
.happy{background-color:yellow}
.twoface{border: solid 1px black;}
</style>
<pre>
                            2020
      January               February               March
Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa
          r1  g2  g3  n4                     G1   n1  n2  n3  n4  n5  n6  n7
 n5  g6  r7  r8  iR9 Y10 g11   g2  y3  y4  g5  n6  r7  g8   n8  n9 n10 n11 n12 n13 n14
g12 R13 n14 r15 iR16 in17 n18   g9 y10 n11 n12 g13 y14 r15  n15 n16 n17 n18 n19 n20 n21
n19 ig20 n21 g22 G23 in24 g25  n16 Y17 r18 n19 n20 n21 n22  n22 n23 n24 n25 n26 n27 n28
ig26 r27 g28 r29 r30 ir31     n23 n24 n25 n26 n27 n28 n29  n29 n30 n31


       April                  May                   June
Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa
          n1  n2  n3  n4                  n1  n2      n1  n2  n3  n4  n5  n6
 n5  n6  n7  n8  n9 n10 n11   n3  n4  n5  n6  n7  n8  n9   n7  n8  n9 n10 n11 n12 n13
n12 n13 n14 n15 n16 n17 n18  n10 n11 n12 n13 n14 n15 n16  n14 n15 n16 n17 n18 n19 n20
n19 n20 n21 n22 n23 n24 n25  n17 n18 n19 n20 n21 n22 n23  n21 n22 n23 n24 n25 n26 n27
n26 n27 n28 n29 n30        n24 n25 n26 n27 n28 n29 n30  n28 n29 n30
                      n31

        July                 August              September
Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa
          n1  n2  n3  n4                     n1         n1  n2  n3  n4  n5
 n5  n6  n7  n8  9 n10 n11   n2  n3  n4  n5  n6  n7  n8   n6  n7  n8  n9 n10 n11 n12
n12 n13 n14 n15 n16 n17 n18   n9 n10 n11 n12 n13 n14 n15  n13 n14 n15 n16 n17 n18 n19
n19 n20 n21 n22 n23 n24 n25  n16 n17 n18 n19 n20 n21 n22  n20 n21 n22 n23 n24 n25 n26
n26 n27 n28 n29 n30 n31     n23 n24 n25 n26 n27 n28 n29  n27 n28 n29 n30
                      n30 n31

      October               November              December
Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa
             n1  n2  n3   n1  n2  n3  n4  n5  n6  n7         n1  n2  n3  n4  n5
 n4  n5  n6  n7  n8  n9 n10   n8  n9 n10 n11 n12 n13 n14   n6  n7  n8  n9 n10 n11 n12
n11 n12 n13 n14 n15 n16 n17  n15 n16 n17 n18 n19 n20 n21  n13 n14 n15 n16 n17 n18 n19
n18 n19 n20 n21 n22 n23 n24  n22 n23 n24 n25 n26 n27 n28  n20 n21 n22 n23 n24 n25 n26
n25 n26 n27 n28 n29 n30 n31  n29 n30                 n27 n28 n29 n30 n31
</pre>
<script>
function colorize(txt, from, to) {
      var regex = new RegExp(from + "([a-zA-Z]*\\d+)", "g");
      return txt.replace(regex, '<span class="' + to + '">$1</span>');
}

var it = document.querySelectorAll('pre')[0].innerText;
it = colorize(it, "i", "twoface");
it = colorize(it, "n", "n");
it = colorize(it, "r", "uneasy");
it = colorize(it, "R", "bad");
it = colorize(it, "g", "nice");
it = colorize(it, "G", "quiteok");
it = colorize(it, "Y", "uneasyandnice");
it = colorize(it, "y", "happy");
document.querySelectorAll('pre')[0].innerHTML = it;
</script>
