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
.twoface{border: solid 4px black;}
</style>
<pre>
                            2020
      January               February               March
Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa
          r1  g2  ig3  n4                     G1   g1  r2  g3  r4  r5  n6  g7
 n5  g6  r7  r8  iR9 Y10 g11   g2  y3  y4  g5  n6  r7  g8   ig8  n9 n10 n11 n12 g13 n14
g12 R13 n14 r15 iR16 in17 n18   g9 y10 n11 n12 g13 iy14 r15  g15 n16 n17 g18 n19 r20 iG21
n19 ig20 n21 g22 G23 in24 g25  n16 iY17 ir18 R19 g20 Y21 ig22  g22 n23 y24 y25 n26 n27 g28
ig26 r27 ig28 r29 r30 ir31     g23 r24 g25 n26 n27 n28 n29  n29 n30 n31


       April                  May                   June
Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa
          n1  n2  n3  n4                  n1  G2      n1  G2  n3  n4  n5  g6
 Y5  n6  g7  n8  n9 r10 y11   g3  g4  n5  n6  n7  n8  n9   g7  g8  n9 n10 n11 n12 n13
g12 r13 r14 g15 g16 r17 R18  n10 n11 n12 n13 n14 G15 Y16  n14 n15 n16 n17 n18 n19 n20
R19 n20 r21 g22 r23 r24 n25  n17 g18 y19 n20 n21 n22 n23  n21 n22 n23 n24 n25 n26 n27
n26 r27 r28 r29 R30        n24 n25 i26 n27 n28 n29 g30  n28 n29 n30
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
