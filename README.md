# daaaaa
1. Aim: To write a Python program for solving the given water-jug problem.
Source Code:
def waterJug(target,ljug,sjug):
jug1=jug2=0
step=1
print(jug1, jug2)
jug2=sjug
step+=1
print(jug1, jug2)
jug1+=jug2
jug2=0
step+=1
print(jug1, jug2)
while jug1!=target:
jug2=0
jug2=sjug
step+=1
print(jug1, jug2)
space=ljug-jug1
if space&lt;=jug2:
jug1+=space
jug2-=space
print(jug1, jug2)
jug1=0
jug1+=jug2
step+=1
else:
jug1+=jug2
jug2=0
step+=1
print(jug1, jug2)
if jug2==target:
jug1=0
step+=1
print(jug1, jug2)
jug1+=jug2
step+=1
jug2=0
break
print(jug1,jug2)
print(&quot;Water in jug1 is: &quot;,jug1)
print(&quot;Number of steps involved are: &quot;,step)
target=int(input(&quot;Enter the target amount of water: &quot;))
ljug=int(input(&quot;Enter the capacity of large jug: &quot;))
sjug=int(input(&quot;Enter the capacity of small jug: &quot;))
print(&quot;The States are: &quot;)
waterJug(target,ljug,sjug)
