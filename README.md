#  Mean and variance of a discrete  distribution


# Aim : 

To find mean and variance of arrival of objects from the feeder using probability distribution


# Software required :  

Python and Visual components tool

# Theory:

The expectation or the mean of a discrete random variable is a weighted average of all possible
values of the random variable. The weights are the probabilities associated with the corresponding values. 
It is calculated as,

![image](https://user-images.githubusercontent.com/103921593/192938463-e34177f4-f188-48a0-bda2-8f6d1d660ed2.png)

The variance of a random variable shows the variability or the scatterings of the random variables.
It shows the distance of a random variable from its mean. It is calcualted as

![image](https://user-images.githubusercontent.com/103921593/192938695-99fedc01-34d5-4d36-84df-5880e766ed0c.png)


# Procedure :

1. Construct frequency distribution for the data

2. Find the  probability distribution from frequency distribution.

3. Calculate mean using 
   
   ![image](https://user-images.githubusercontent.com/103921593/192940431-03b81777-c54d-4286-b4f4-82dfe7666b4c.png)

4. Find  
   
      ![image](https://user-images.githubusercontent.com/103921593/192940255-2d9dd746-6875-4a6d-877b-6da6cdb96ab1.png)

5.  Calculate variance using 
  
      ![image](https://user-images.githubusercontent.com/103921593/192942852-913550a9-fabe-4a55-b956-0487b18bbd97.png)


# Experiment :

![Visual Component](https://user-images.githubusercontent.com/93427182/192949045-d865cdf6-88ee-4ec8-a60b-295dd233dfcc.PNG)

# Program :
~~~
Developed By : Shyam Kumar A
Reg No :212221230098
~~~
~~~
import humpy as np
L=[int (i) for i in input () .split ()]
N=1en (L) ; M=max (L)
x=list ();f=list ()
for i in range (M+1) :
   c = 0
   for j in range (N) :
      if L[j]==i:
         c=c+1
   f.append(c)
   x.append(i)
sf=np.sum(f)
p=list()
for i in range (M+1) :
   p-append(f[i]/sf)
mean=p-inner(x,p)
EX2=np-inner (np. square (x), P)
var=EX2-mean**2
SD=np.sqrt(var)
print("The Hean arrival rate is %.3f "%mean)
print ("The Variance of arrival from feeder is %.3f"%var)
print ("The Standard deviation of arrival from feeder is %.3F"%SD)
~~~
# Results and Output : 
![Output](https://user-images.githubusercontent.com/93427182/192949486-823933ae-c7e1-4c3e-838c-f9a54b6d2c8d.png)
