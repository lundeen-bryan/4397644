# DataFrame Basics Exercise

## Part 1
* Use pandas to read the `bestsellers` dataset into a DataFrame 
* Once you've done that, use Pandas to figure out how many rows and columns the DF has
* Inspect the first 5 rows
* Inspect the first 19 rows
* Inspect the last 5 rows
* Inspect the last 2 rows 
* Which columns (if any) are missing values?
* What datatype did Pandas assign to "User Rating"?
* How many integer columns are in the DataFrame?


```python
import pandas as pd
```


```python
books = pd.read_csv("./../data/bestsellers.csv")
books
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Author</th>
      <th>User Rating</th>
      <th>Reviews</th>
      <th>Price</th>
      <th>Year</th>
      <th>Genre</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>10-Day Green Smoothie Cleanse</td>
      <td>JJ Smith</td>
      <td>4.7</td>
      <td>17350</td>
      <td>8</td>
      <td>2016</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>1</th>
      <td>11/22/63: A Novel</td>
      <td>Stephen King</td>
      <td>4.6</td>
      <td>2052</td>
      <td>22</td>
      <td>2011</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>2</th>
      <td>12 Rules for Life: An Antidote to Chaos</td>
      <td>Jordan B. Peterson</td>
      <td>4.7</td>
      <td>18979</td>
      <td>15</td>
      <td>2018</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1984 (Signet Classics)</td>
      <td>George Orwell</td>
      <td>4.7</td>
      <td>21424</td>
      <td>6</td>
      <td>2017</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5,000 Awesome Facts (About Everything!) (Natio...</td>
      <td>National Geographic Kids</td>
      <td>4.8</td>
      <td>7665</td>
      <td>12</td>
      <td>2019</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>545</th>
      <td>Wrecking Ball (Diary of a Wimpy Kid Book 14)</td>
      <td>Jeff Kinney</td>
      <td>4.9</td>
      <td>9413</td>
      <td>8</td>
      <td>2019</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>546</th>
      <td>You Are a Badass: How to Stop Doubting Your Gr...</td>
      <td>Jen Sincero</td>
      <td>4.7</td>
      <td>14331</td>
      <td>8</td>
      <td>2016</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>547</th>
      <td>You Are a Badass: How to Stop Doubting Your Gr...</td>
      <td>Jen Sincero</td>
      <td>4.7</td>
      <td>14331</td>
      <td>8</td>
      <td>2017</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>548</th>
      <td>You Are a Badass: How to Stop Doubting Your Gr...</td>
      <td>Jen Sincero</td>
      <td>4.7</td>
      <td>14331</td>
      <td>8</td>
      <td>2018</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>549</th>
      <td>You Are a Badass: How to Stop Doubting Your Gr...</td>
      <td>Jen Sincero</td>
      <td>4.7</td>
      <td>14331</td>
      <td>8</td>
      <td>2019</td>
      <td>Non Fiction</td>
    </tr>
  </tbody>
</table>
<p>550 rows × 7 columns</p>
</div>




```python
# Inspect the first 5 rows
books.head(5)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Author</th>
      <th>User Rating</th>
      <th>Reviews</th>
      <th>Price</th>
      <th>Year</th>
      <th>Genre</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>10-Day Green Smoothie Cleanse</td>
      <td>JJ Smith</td>
      <td>4.7</td>
      <td>17350</td>
      <td>8</td>
      <td>2016</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>1</th>
      <td>11/22/63: A Novel</td>
      <td>Stephen King</td>
      <td>4.6</td>
      <td>2052</td>
      <td>22</td>
      <td>2011</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>2</th>
      <td>12 Rules for Life: An Antidote to Chaos</td>
      <td>Jordan B. Peterson</td>
      <td>4.7</td>
      <td>18979</td>
      <td>15</td>
      <td>2018</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1984 (Signet Classics)</td>
      <td>George Orwell</td>
      <td>4.7</td>
      <td>21424</td>
      <td>6</td>
      <td>2017</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5,000 Awesome Facts (About Everything!) (Natio...</td>
      <td>National Geographic Kids</td>
      <td>4.8</td>
      <td>7665</td>
      <td>12</td>
      <td>2019</td>
      <td>Non Fiction</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Inspect the first 19 rows
books.head(19)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Author</th>
      <th>User Rating</th>
      <th>Reviews</th>
      <th>Price</th>
      <th>Year</th>
      <th>Genre</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>10-Day Green Smoothie Cleanse</td>
      <td>JJ Smith</td>
      <td>4.7</td>
      <td>17350</td>
      <td>8</td>
      <td>2016</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>1</th>
      <td>11/22/63: A Novel</td>
      <td>Stephen King</td>
      <td>4.6</td>
      <td>2052</td>
      <td>22</td>
      <td>2011</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>2</th>
      <td>12 Rules for Life: An Antidote to Chaos</td>
      <td>Jordan B. Peterson</td>
      <td>4.7</td>
      <td>18979</td>
      <td>15</td>
      <td>2018</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1984 (Signet Classics)</td>
      <td>George Orwell</td>
      <td>4.7</td>
      <td>21424</td>
      <td>6</td>
      <td>2017</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5,000 Awesome Facts (About Everything!) (Natio...</td>
      <td>National Geographic Kids</td>
      <td>4.8</td>
      <td>7665</td>
      <td>12</td>
      <td>2019</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>5</th>
      <td>A Dance with Dragons (A Song of Ice and Fire)</td>
      <td>George R. R. Martin</td>
      <td>4.4</td>
      <td>12643</td>
      <td>11</td>
      <td>2011</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>6</th>
      <td>A Game of Thrones / A Clash of Kings / A Storm...</td>
      <td>George R. R. Martin</td>
      <td>4.7</td>
      <td>19735</td>
      <td>30</td>
      <td>2014</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>7</th>
      <td>A Gentleman in Moscow: A Novel</td>
      <td>Amor Towles</td>
      <td>4.7</td>
      <td>19699</td>
      <td>15</td>
      <td>2017</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>8</th>
      <td>A Higher Loyalty: Truth, Lies, and Leadership</td>
      <td>James Comey</td>
      <td>4.7</td>
      <td>5983</td>
      <td>3</td>
      <td>2018</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>9</th>
      <td>A Man Called Ove: A Novel</td>
      <td>Fredrik Backman</td>
      <td>4.6</td>
      <td>23848</td>
      <td>8</td>
      <td>2016</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>10</th>
      <td>A Man Called Ove: A Novel</td>
      <td>Fredrik Backman</td>
      <td>4.6</td>
      <td>23848</td>
      <td>8</td>
      <td>2017</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>11</th>
      <td>A Patriot's History of the United States: From...</td>
      <td>Larry Schweikart</td>
      <td>4.6</td>
      <td>460</td>
      <td>2</td>
      <td>2010</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>12</th>
      <td>A Stolen Life: A Memoir</td>
      <td>Jaycee Dugard</td>
      <td>4.6</td>
      <td>4149</td>
      <td>32</td>
      <td>2011</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>13</th>
      <td>A Wrinkle in Time (Time Quintet)</td>
      <td>Madeleine L'Engle</td>
      <td>4.5</td>
      <td>5153</td>
      <td>5</td>
      <td>2018</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Act Like a Lady, Think Like a Man: What Men Re...</td>
      <td>Steve Harvey</td>
      <td>4.6</td>
      <td>5013</td>
      <td>17</td>
      <td>2009</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>15</th>
      <td>Adult Coloring Book Designs: Stress Relief Col...</td>
      <td>Adult Coloring Book Designs</td>
      <td>4.5</td>
      <td>2313</td>
      <td>4</td>
      <td>2016</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Adult Coloring Book: Stress Relieving Animal D...</td>
      <td>Blue Star Coloring</td>
      <td>4.6</td>
      <td>2925</td>
      <td>6</td>
      <td>2015</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Adult Coloring Book: Stress Relieving Patterns</td>
      <td>Blue Star Coloring</td>
      <td>4.4</td>
      <td>2951</td>
      <td>6</td>
      <td>2015</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Adult Coloring Books: A Coloring Book for Adul...</td>
      <td>Coloring Books for Adults</td>
      <td>4.5</td>
      <td>2426</td>
      <td>8</td>
      <td>2015</td>
      <td>Non Fiction</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Inspect the last 5 rows
books.tail(5)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Author</th>
      <th>User Rating</th>
      <th>Reviews</th>
      <th>Price</th>
      <th>Year</th>
      <th>Genre</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>545</th>
      <td>Wrecking Ball (Diary of a Wimpy Kid Book 14)</td>
      <td>Jeff Kinney</td>
      <td>4.9</td>
      <td>9413</td>
      <td>8</td>
      <td>2019</td>
      <td>Fiction</td>
    </tr>
    <tr>
      <th>546</th>
      <td>You Are a Badass: How to Stop Doubting Your Gr...</td>
      <td>Jen Sincero</td>
      <td>4.7</td>
      <td>14331</td>
      <td>8</td>
      <td>2016</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>547</th>
      <td>You Are a Badass: How to Stop Doubting Your Gr...</td>
      <td>Jen Sincero</td>
      <td>4.7</td>
      <td>14331</td>
      <td>8</td>
      <td>2017</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>548</th>
      <td>You Are a Badass: How to Stop Doubting Your Gr...</td>
      <td>Jen Sincero</td>
      <td>4.7</td>
      <td>14331</td>
      <td>8</td>
      <td>2018</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>549</th>
      <td>You Are a Badass: How to Stop Doubting Your Gr...</td>
      <td>Jen Sincero</td>
      <td>4.7</td>
      <td>14331</td>
      <td>8</td>
      <td>2019</td>
      <td>Non Fiction</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Inspect the last 2 rows 
books.tail(2)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Author</th>
      <th>User Rating</th>
      <th>Reviews</th>
      <th>Price</th>
      <th>Year</th>
      <th>Genre</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>548</th>
      <td>You Are a Badass: How to Stop Doubting Your Gr...</td>
      <td>Jen Sincero</td>
      <td>4.7</td>
      <td>14331</td>
      <td>8</td>
      <td>2018</td>
      <td>Non Fiction</td>
    </tr>
    <tr>
      <th>549</th>
      <td>You Are a Badass: How to Stop Doubting Your Gr...</td>
      <td>Jen Sincero</td>
      <td>4.7</td>
      <td>14331</td>
      <td>8</td>
      <td>2019</td>
      <td>Non Fiction</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Which columns (if any) are missing values?
books.info()
# result = no missing values
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 550 entries, 0 to 549
    Data columns (total 7 columns):
     #   Column       Non-Null Count  Dtype  
    ---  ------       --------------  -----  
     0   Name         550 non-null    object 
     1   Author       550 non-null    object 
     2   User Rating  550 non-null    float64
     3   Reviews      550 non-null    int64  
     4   Price        550 non-null    int64  
     5   Year         550 non-null    int64  
     6   Genre        550 non-null    object 
    dtypes: float64(1), int64(3), object(3)
    memory usage: 30.2+ KB
    


```python
# What datatype did Pandas assign to "User Rating"?
# ans = float
books["User Rating"].dtype
```




    dtype('float64')




```python
# How many integer columns are in the DataFrame?
# ans = 3 
books.select_dtypes(include=['int']).info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 550 entries, 0 to 549
    Data columns (total 3 columns):
     #   Column   Non-Null Count  Dtype
    ---  ------   --------------  -----
     0   Reviews  550 non-null    int64
     1   Price    550 non-null    int64
     2   Year     550 non-null    int64
    dtypes: int64(3)
    memory usage: 13.0 KB
    

## Part 2

* The `mount_everest_deaths` dataset has its own index column provided in the dataset.  When importing it, use the existing index column.
* Which columns have zero null values?
* Which column has the most null values?



```python
# The `mount_everest_deaths` dataset has its own index column provided
# in the dataset.  When importing it, use the existing index column.
mnt = pd.read_csv("./../data/mount_everest_deaths.csv").set_index("No.")
mnt
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Date</th>
      <th>Age</th>
      <th>Expedition</th>
      <th>Nationality</th>
      <th>Cause of death</th>
      <th>Location</th>
    </tr>
    <tr>
      <th>No.</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>Dorje</td>
      <td>June 7, 1922</td>
      <td>NaN</td>
      <td>1922 British Mount Everest Expedition</td>
      <td>Nepal</td>
      <td>Avalanche</td>
      <td>Below North Col</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Lhakpa</td>
      <td>June 7, 1922</td>
      <td>NaN</td>
      <td>1922 British Mount Everest Expedition</td>
      <td>Nepal</td>
      <td>Avalanche</td>
      <td>Below North Col</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Norbu</td>
      <td>June 7, 1922</td>
      <td>NaN</td>
      <td>1922 British Mount Everest Expedition</td>
      <td>Nepal</td>
      <td>Avalanche</td>
      <td>Below North Col</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Pasang</td>
      <td>June 7, 1922</td>
      <td>NaN</td>
      <td>1922 British Mount Everest Expedition</td>
      <td>Nepal</td>
      <td>Avalanche</td>
      <td>Below North Col</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Pema</td>
      <td>June 7, 1922</td>
      <td>NaN</td>
      <td>1922 British Mount Everest Expedition</td>
      <td>Nepal</td>
      <td>Avalanche</td>
      <td>Below North Col</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>306</th>
      <td>Christopher Jon Kulish</td>
      <td>May 27, 2019</td>
      <td>62.0</td>
      <td>Climbing the Seven Summits</td>
      <td>United States</td>
      <td>Cardiac event during descent</td>
      <td>South Col</td>
    </tr>
    <tr>
      <th>307</th>
      <td>Puwei Liu</td>
      <td>May 12, 2021</td>
      <td>55.0</td>
      <td>Seven Summit Treks</td>
      <td>United States</td>
      <td>Exhaustion</td>
      <td>Near South Summit</td>
    </tr>
    <tr>
      <th>308</th>
      <td>Abdul Waraich</td>
      <td>May 12, 2021</td>
      <td>41.0</td>
      <td>Seven Summit Treks</td>
      <td>Switzerland</td>
      <td>Exhaustion</td>
      <td>Near South Summit</td>
    </tr>
    <tr>
      <th>309</th>
      <td>Pemba Tashi Sherpa</td>
      <td>May 18, 2021</td>
      <td>28.0</td>
      <td>Climbing the Seven Summits</td>
      <td>Nepal</td>
      <td>Fall into a crevasse</td>
      <td>Between Camp I &amp; Camp II</td>
    </tr>
    <tr>
      <th>310</th>
      <td>Wong Dorchi Sherpa</td>
      <td>May 23, 2021</td>
      <td>NaN</td>
      <td>7 Summits Club</td>
      <td>Nepal</td>
      <td>NaN</td>
      <td>near South Col</td>
    </tr>
  </tbody>
</table>
<p>310 rows × 7 columns</p>
</div>




```python
# Which columns have zero null values?
## check if there are any null values in any column
mnt.isnull().any()
## if returns true then we have some null values in the column

```




    Name              False
    Date              False
    Age                True
    Expedition         True
    Nationality        True
    Cause of death     True
    Location           True
    dtype: bool




```python
## show count of values in each column that are null
mnt.isnull().sum()

```




    Name                0
    Date                0
    Age               150
    Expedition         39
    Nationality         1
    Cause of death     14
    Location           19
    dtype: int64




```python
## double-check if there are any non-null values
mnt.notnull().sum()

```




    Name              310
    Date              310
    Age               160
    Expedition        271
    Nationality       309
    Cause of death    296
    Location          291
    dtype: int64




```python
# Which column has the most null values?
mnt.isnull().sum().idxmax()
```




    'Age'



## Part 3
* Import the `movie_titles.tsv` dataset
* You'll notice that it is not comma-separated! You'll need to tell `read_csv` what the separator actually is.
* The dataset does not come with its own column headings, so you'll need to provide those as well.  The columns are, in order, `id`, `title`, `year`, `imdb_rating`, `imdb_id`, and `genres`
* Once you have successfully read the dataset into a DataFrame, inspect the last 7 rows!


```python
# Import the `movie_titles.tsv` dataset You'll notice that it is not
# comma-separated! You'll need to tell `read_csv` what the separator
# actually is.
mov = pd.read_csv("./../data/movie_titles.tsv", sep="\t")
mov
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>m0</th>
      <th>10 things i hate about you</th>
      <th>1999</th>
      <th>6.90</th>
      <th>62847</th>
      <th>['comedy' 'romance']</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>m1</td>
      <td>1492: conquest of paradise</td>
      <td>1992</td>
      <td>6.2</td>
      <td>10421.0</td>
      <td>['adventure' 'biography' 'drama' 'history']</td>
    </tr>
    <tr>
      <th>1</th>
      <td>m2</td>
      <td>15 minutes</td>
      <td>2001</td>
      <td>6.1</td>
      <td>25854.0</td>
      <td>['action' 'crime' 'drama' 'thriller']</td>
    </tr>
    <tr>
      <th>2</th>
      <td>m3</td>
      <td>2001: a space odyssey</td>
      <td>1968</td>
      <td>8.4</td>
      <td>163227.0</td>
      <td>['adventure' 'mystery' 'sci-fi']</td>
    </tr>
    <tr>
      <th>3</th>
      <td>m4</td>
      <td>48 hrs.</td>
      <td>1982</td>
      <td>6.9</td>
      <td>22289.0</td>
      <td>['action' 'comedy' 'crime' 'drama' 'thriller']</td>
    </tr>
    <tr>
      <th>4</th>
      <td>m5</td>
      <td>the fifth element</td>
      <td>1997</td>
      <td>7.5</td>
      <td>133756.0</td>
      <td>['action' 'adventure' 'romance' 'sci-fi' 'thri...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>611</th>
      <td>m612</td>
      <td>watchmen</td>
      <td>2009</td>
      <td>7.8</td>
      <td>135229.0</td>
      <td>['action' 'crime' 'fantasy' 'mystery' 'sci-fi'...</td>
    </tr>
    <tr>
      <th>612</th>
      <td>m613</td>
      <td>xxx</td>
      <td>2002</td>
      <td>5.6</td>
      <td>53505.0</td>
      <td>['action' 'adventure' 'crime']</td>
    </tr>
    <tr>
      <th>613</th>
      <td>m614</td>
      <td>x-men</td>
      <td>2000</td>
      <td>7.4</td>
      <td>122149.0</td>
      <td>['action' 'sci-fi']</td>
    </tr>
    <tr>
      <th>614</th>
      <td>m615</td>
      <td>young frankenstein</td>
      <td>1974</td>
      <td>8.0</td>
      <td>57618.0</td>
      <td>['comedy' 'sci-fi']</td>
    </tr>
    <tr>
      <th>615</th>
      <td>m616</td>
      <td>zulu dawn</td>
      <td>1979</td>
      <td>6.4</td>
      <td>1911.0</td>
      <td>['action' 'adventure' 'drama' 'history' 'war']</td>
    </tr>
  </tbody>
</table>
<p>616 rows × 6 columns</p>
</div>




```python
# The dataset does not come with its own column headings, so you'll need
# to provide those as well.  The columns are, in order, `id`, `title`,
# `year`, `imdb_rating`, `imdb_id`, and `genres`
## create list of headings
headings = ["id", "title","year", "imdb_rating", "imdb_id", "genres"]
## set column heading names
mov.columns = headings
## set new index for dataframe; use "inplace" keyword bcuz the df was previously created
mov.set_index("id", inplace=True)
mov

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>title</th>
      <th>year</th>
      <th>imdb_rating</th>
      <th>imdb_id</th>
      <th>genres</th>
    </tr>
    <tr>
      <th>id</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>m1</th>
      <td>1492: conquest of paradise</td>
      <td>1992</td>
      <td>6.2</td>
      <td>10421.0</td>
      <td>['adventure' 'biography' 'drama' 'history']</td>
    </tr>
    <tr>
      <th>m2</th>
      <td>15 minutes</td>
      <td>2001</td>
      <td>6.1</td>
      <td>25854.0</td>
      <td>['action' 'crime' 'drama' 'thriller']</td>
    </tr>
    <tr>
      <th>m3</th>
      <td>2001: a space odyssey</td>
      <td>1968</td>
      <td>8.4</td>
      <td>163227.0</td>
      <td>['adventure' 'mystery' 'sci-fi']</td>
    </tr>
    <tr>
      <th>m4</th>
      <td>48 hrs.</td>
      <td>1982</td>
      <td>6.9</td>
      <td>22289.0</td>
      <td>['action' 'comedy' 'crime' 'drama' 'thriller']</td>
    </tr>
    <tr>
      <th>m5</th>
      <td>the fifth element</td>
      <td>1997</td>
      <td>7.5</td>
      <td>133756.0</td>
      <td>['action' 'adventure' 'romance' 'sci-fi' 'thri...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>m612</th>
      <td>watchmen</td>
      <td>2009</td>
      <td>7.8</td>
      <td>135229.0</td>
      <td>['action' 'crime' 'fantasy' 'mystery' 'sci-fi'...</td>
    </tr>
    <tr>
      <th>m613</th>
      <td>xxx</td>
      <td>2002</td>
      <td>5.6</td>
      <td>53505.0</td>
      <td>['action' 'adventure' 'crime']</td>
    </tr>
    <tr>
      <th>m614</th>
      <td>x-men</td>
      <td>2000</td>
      <td>7.4</td>
      <td>122149.0</td>
      <td>['action' 'sci-fi']</td>
    </tr>
    <tr>
      <th>m615</th>
      <td>young frankenstein</td>
      <td>1974</td>
      <td>8.0</td>
      <td>57618.0</td>
      <td>['comedy' 'sci-fi']</td>
    </tr>
    <tr>
      <th>m616</th>
      <td>zulu dawn</td>
      <td>1979</td>
      <td>6.4</td>
      <td>1911.0</td>
      <td>['action' 'adventure' 'drama' 'history' 'war']</td>
    </tr>
  </tbody>
</table>
<p>616 rows × 5 columns</p>
</div>


