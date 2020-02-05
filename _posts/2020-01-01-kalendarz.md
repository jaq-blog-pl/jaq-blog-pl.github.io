---
layout: post
title: "Kalendarz"
date: 2020-01-01
---

Czy jest lepiej czy jest źlej?

<style>
.bigred{background-color:red}
.red{background-color:#ffaaaa}
.green{background-color:green}
.smallgreen{background-color:#aaffaa}
.redandgreen{background-image: linear-gradient(to bottom right, #ffaaaa 0%, #ffaaaa 50%, green 50%, green 100%);}
.yellow{background-color:yellow}
</style>
<pre>
                            2020
      January               February               March          
Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  Su Mo Tu We Th Fr Sa  
          r1  g2  g3  n4                     G1   n1  n2  n3  n4  n5  n6  n7
 n5  g6  r7  r8  R9 Y10 g11   g2  n3  n4  y5  n6  n7  n8   n8  n9 n10 n11 n12 n13 n14
g12 R13 n14 r15 R16 n17 n18   n9 n10 n11 n12 n13 n14 n15  n15 n16 n17 n18 n19 n20 n21  
n19 g20 n21 g22 G23 n24 g25  n16 n17 n18 n19 n20 n21 n22  n22 n23 n24 n25 n26 n27 n28  
g26 r27 g28 r29 r30 r31     n23 n24 n25 n26 n27 n28 n29  n29 n30 n31
                                                                  

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
 n5  n6  n7  n8  n9 n10 n11   n2  n3  n4  n5  n6  n7  n8   n6  n7  n8  n9 n10 n11 n12  
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
var it = document.querySelectorAll('pre')[0].innerText;
it = it.replace(/n(\d+)/g, '<span class="n">$1</span>');
it = it.replace(/r(\d+)/g, '<span class="red">$1</span>');
it = it.replace(/R(\d+)/g, '<span class="bigred">$1</span>');
it = it.replace(/g(\d+)/g, '<span class="green">$1</span>');
it = it.replace(/G(\d+)/g, '<span class="smallgreen">$1</span>');
it = it.replace(/Y(\d+)/g, '<span class="redandgreen">$1</span>');
it = it.replace(/y(\d+)/g, '<span class="yellow">$1</span>');
document.querySelectorAll('pre')[0].innerHTML = it;
</script>
