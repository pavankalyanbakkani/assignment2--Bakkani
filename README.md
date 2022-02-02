# assignment2--Bakkani
# Pavan kalyan Bakkani
###### Fire&Ice Restaurant
We do have **coffee shop** right opposite it and The **Drive In** in the Backyard and Trends and Marts to both the sides of  it.


---

### Directions to the food place

RGIA International Airport-Shamshabad

1. Hire a taxi from airport to golconda fort,Suncity via  Nehru ORR-Outer Ring Road Lane.
2. Probably, it takes 30 min to reach the food place.
3. Will find the place  exactly at the Gas station and  opposite to the Coffee Shop.

##### I recommend to taste the below mentioned

* Non-Veg
    
    * Hyderabad Chicken Dum Biryani
    * Hyderabad Special Chicken Dum Biryani
    * Hyderabad Mutton Dum Biryani
    * Hyderabad Mutton keema Dum Biryani

* Veg

    * Butter Naan
    * Roti
    * Paneer Biryani

* Drinks

     * Coca Cola 


[link to AboutMe](AboutMe.md)




----

# Sports Activity Table

The following table represents the Sports Activities that someone can lookup on their interest.

|Sport|Location|Cost|    
|---|---|---|
|Cricket|Endland|100$|
|Baseball|USA|1k$|
|Hockey|india|70$|
|Badminton|Australia|70$|


----

# Pithy Quotes
>  "Therefore do not worry about tomorrow, for tomorrow will worry about itself. Each day has enough trouble of its own" -*Matthew*

> “The righteous will live by faith.”  -*Romans*


---

# Code fencing

> Sparse table concept is used for fast queries on a set of static data (elements do not change). It does preprocessing so that the queries can be answered efficiently.

Link to source <https://www.geeksforgeeks.org/sparse-table/?ref=gcse>

```
Precomputation:

for (int i = 0; i < N; i++)
    st[i][0] = f(array[i]);

for (int j = 1; j <= K; j++)
    for (int i = 0; i + (1 << j) <= N; i++)
        st[i][j] = f(st[i][j-1], st[i + (1 << (j - 1))][j - 1]);

Range Sum Queries:

long long st[MAXN][K + 1];

for (int i = 0; i < N; i++)
    st[i][0] = array[i];

for (int j = 1; j <= K; j++)
    for (int i = 0; i + (1 << j) <= N; i++)
        st[i][j] = st[i][j-1] + st[i + (1 << (j - 1))][j - 1];

Range Minimum Queries (RMQ):

int log[MAXN+1];
log[1] = 0;
for (int i = 2; i <= MAXN; i++)
    log[i] = log[i/2] + 1;

int st[MAXN][K + 1];

for (int i = 0; i < N; i++)
    st[i][0] = array[i];

for (int j = 1; j <= K; j++)
    for (int i = 0; i + (1 << j) <= N; i++)
        st[i][j] = min(st[i][j-1], st[i + (1 << (j - 1))][j - 1]);

```

Link to source code <https://cp-algorithms.com/data_structures/sparse-table.html>


