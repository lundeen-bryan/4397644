# DataFrames Basics


```python
import pandas as pd
```

The `read_csv` method will read in a CSV file and returns to us a DataFrame


```python
states = pd.read_csv("data/states.csv")
states
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
      <th>State</th>
      <th>Abbrev</th>
      <th>Code</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Alabama</td>
      <td>Ala.</td>
      <td>AL</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Alaska</td>
      <td>Alaska</td>
      <td>AK</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Arizona</td>
      <td>Ariz.</td>
      <td>AZ</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Arkansas</td>
      <td>Ark.</td>
      <td>AR</td>
    </tr>
    <tr>
      <th>4</th>
      <td>California</td>
      <td>Calif.</td>
      <td>CA</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Colorado</td>
      <td>Colo.</td>
      <td>CO</td>
    </tr>
    <tr>
      <th>6</th>
      <td>Connecticut</td>
      <td>Conn.</td>
      <td>CT</td>
    </tr>
    <tr>
      <th>7</th>
      <td>Delaware</td>
      <td>Del.</td>
      <td>DE</td>
    </tr>
    <tr>
      <th>8</th>
      <td>District of Columbia</td>
      <td>D.C.</td>
      <td>DC</td>
    </tr>
    <tr>
      <th>9</th>
      <td>Florida</td>
      <td>Fla.</td>
      <td>FL</td>
    </tr>
    <tr>
      <th>10</th>
      <td>Georgia</td>
      <td>Ga.</td>
      <td>GA</td>
    </tr>
    <tr>
      <th>11</th>
      <td>Hawaii</td>
      <td>Hawaii</td>
      <td>HI</td>
    </tr>
    <tr>
      <th>12</th>
      <td>Idaho</td>
      <td>Idaho</td>
      <td>ID</td>
    </tr>
    <tr>
      <th>13</th>
      <td>Illinois</td>
      <td>Ill.</td>
      <td>IL</td>
    </tr>
    <tr>
      <th>14</th>
      <td>Indiana</td>
      <td>Ind.</td>
      <td>IN</td>
    </tr>
    <tr>
      <th>15</th>
      <td>Iowa</td>
      <td>Iowa</td>
      <td>IA</td>
    </tr>
    <tr>
      <th>16</th>
      <td>Kansas</td>
      <td>Kans.</td>
      <td>KS</td>
    </tr>
    <tr>
      <th>17</th>
      <td>Kentucky</td>
      <td>Ky.</td>
      <td>KY</td>
    </tr>
    <tr>
      <th>18</th>
      <td>Louisiana</td>
      <td>La.</td>
      <td>LA</td>
    </tr>
    <tr>
      <th>19</th>
      <td>Maine</td>
      <td>Maine</td>
      <td>ME</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Maryland</td>
      <td>Md.</td>
      <td>MD</td>
    </tr>
    <tr>
      <th>21</th>
      <td>Massachusetts</td>
      <td>Mass.</td>
      <td>MA</td>
    </tr>
    <tr>
      <th>22</th>
      <td>Michigan</td>
      <td>Mich.</td>
      <td>MI</td>
    </tr>
    <tr>
      <th>23</th>
      <td>Minnesota</td>
      <td>Minn.</td>
      <td>MN</td>
    </tr>
    <tr>
      <th>24</th>
      <td>Mississippi</td>
      <td>Miss.</td>
      <td>MS</td>
    </tr>
    <tr>
      <th>25</th>
      <td>Missouri</td>
      <td>Mo.</td>
      <td>MO</td>
    </tr>
    <tr>
      <th>26</th>
      <td>Montana</td>
      <td>Mont.</td>
      <td>MT</td>
    </tr>
    <tr>
      <th>27</th>
      <td>Nebraska</td>
      <td>Nebr.</td>
      <td>NE</td>
    </tr>
    <tr>
      <th>28</th>
      <td>Nevada</td>
      <td>Nev.</td>
      <td>NV</td>
    </tr>
    <tr>
      <th>29</th>
      <td>New Hampshire</td>
      <td>N.H.</td>
      <td>NH</td>
    </tr>
    <tr>
      <th>30</th>
      <td>New Jersey</td>
      <td>N.J.</td>
      <td>NJ</td>
    </tr>
    <tr>
      <th>31</th>
      <td>New Mexico</td>
      <td>N.M.</td>
      <td>NM</td>
    </tr>
    <tr>
      <th>32</th>
      <td>New York</td>
      <td>N.Y.</td>
      <td>NY</td>
    </tr>
    <tr>
      <th>33</th>
      <td>North Carolina</td>
      <td>N.C.</td>
      <td>NC</td>
    </tr>
    <tr>
      <th>34</th>
      <td>North Dakota</td>
      <td>N.D.</td>
      <td>ND</td>
    </tr>
    <tr>
      <th>35</th>
      <td>Ohio</td>
      <td>Ohio</td>
      <td>OH</td>
    </tr>
    <tr>
      <th>36</th>
      <td>Oklahoma</td>
      <td>Okla.</td>
      <td>OK</td>
    </tr>
    <tr>
      <th>37</th>
      <td>Oregon</td>
      <td>Ore.</td>
      <td>OR</td>
    </tr>
    <tr>
      <th>38</th>
      <td>Pennsylvania</td>
      <td>Pa.</td>
      <td>PA</td>
    </tr>
    <tr>
      <th>39</th>
      <td>Rhode Island</td>
      <td>R.I.</td>
      <td>RI</td>
    </tr>
    <tr>
      <th>40</th>
      <td>South Carolina</td>
      <td>S.C.</td>
      <td>SC</td>
    </tr>
    <tr>
      <th>41</th>
      <td>South Dakota</td>
      <td>S.D.</td>
      <td>SD</td>
    </tr>
    <tr>
      <th>42</th>
      <td>Tennessee</td>
      <td>Tenn.</td>
      <td>TN</td>
    </tr>
    <tr>
      <th>43</th>
      <td>Texas</td>
      <td>Tex.</td>
      <td>TX</td>
    </tr>
    <tr>
      <th>44</th>
      <td>Utah</td>
      <td>Utah</td>
      <td>UT</td>
    </tr>
    <tr>
      <th>45</th>
      <td>Vermont</td>
      <td>Vt.</td>
      <td>VT</td>
    </tr>
    <tr>
      <th>46</th>
      <td>Virginia</td>
      <td>Va.</td>
      <td>VA</td>
    </tr>
    <tr>
      <th>47</th>
      <td>Washington</td>
      <td>Wash.</td>
      <td>WA</td>
    </tr>
    <tr>
      <th>48</th>
      <td>West Virginia</td>
      <td>W.Va.</td>
      <td>WV</td>
    </tr>
    <tr>
      <th>49</th>
      <td>Wisconsin</td>
      <td>Wis.</td>
      <td>WI</td>
    </tr>
    <tr>
      <th>50</th>
      <td>Wyoming</td>
      <td>Wyo.</td>
      <td>WY</td>
    </tr>
  </tbody>
</table>
</div>



## King County Home Sales Data Set
This dataset includes the home sales from 2014-2015 in King County, WA (the county Seattle is located in)
* `id` - house's unique id
* `date` - sale date
* `price` - sale price
* `bedrooms` - number of bedrooms
* `bathrooms` - numbers of bathrooms
* `sqft_living` - living space square footage 
* `sqft_lot` - total lot square footage
* `floors` - numbers of floors
* `waterfront` - is the house waterfront (1) or not (0)
* `view` - rating from 0 to 4 of how good the view from the house is
* `condition` - rating from 1 (poor) to 5 (very good) of the condition of the house
* `grade` - rating from 1-13 representing the construction quality of improvements. 1-3 Falls short of minimum building standards (cabins, etc.) 7 is avg grade, 11-13 have high-quality design & construction
* `sqft_above` - square footage of the interior that is above ground level
* `sqft_basement` - square footage of the interior that is below ground level
* `yr_built` - year the house was initially built
* `yr_renovated` - The year of the house’s last renovation (if any)
* `zipcode` - zipcode that the house is located in
* `lat` - the property's latitude
* `long` - the property's longitude
* `sqft_living15` - average interior space square footage of the nearest 15 neighbors
* `sqft_lot15` - average lot square footage of the nearest 15 neighbors


```python
houses = pd.read_csv("data/kc_house_data.csv")
```


```python
houses.head()
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
      <th>id</th>
      <th>date</th>
      <th>price</th>
      <th>bedrooms</th>
      <th>bathrooms</th>
      <th>sqft_living</th>
      <th>sqft_lot</th>
      <th>floors</th>
      <th>waterfront</th>
      <th>view</th>
      <th>...</th>
      <th>grade</th>
      <th>sqft_above</th>
      <th>sqft_basement</th>
      <th>yr_built</th>
      <th>yr_renovated</th>
      <th>zipcode</th>
      <th>lat</th>
      <th>long</th>
      <th>sqft_living15</th>
      <th>sqft_lot15</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>7129300520</td>
      <td>20141013T000000</td>
      <td>221900.0</td>
      <td>3</td>
      <td>1.00</td>
      <td>1180</td>
      <td>5650</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1180</td>
      <td>0</td>
      <td>1955</td>
      <td>0</td>
      <td>98178</td>
      <td>47.5112</td>
      <td>-122.257</td>
      <td>1340</td>
      <td>5650</td>
    </tr>
    <tr>
      <th>1</th>
      <td>6414100192</td>
      <td>20141209T000000</td>
      <td>538000.0</td>
      <td>3</td>
      <td>2.25</td>
      <td>2570</td>
      <td>7242</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>2170</td>
      <td>400</td>
      <td>1951</td>
      <td>1991</td>
      <td>98125</td>
      <td>47.7210</td>
      <td>-122.319</td>
      <td>1690</td>
      <td>7639</td>
    </tr>
    <tr>
      <th>2</th>
      <td>5631500400</td>
      <td>20150225T000000</td>
      <td>180000.0</td>
      <td>2</td>
      <td>1.00</td>
      <td>770</td>
      <td>10000</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>6</td>
      <td>770</td>
      <td>0</td>
      <td>1933</td>
      <td>0</td>
      <td>98028</td>
      <td>47.7379</td>
      <td>-122.233</td>
      <td>2720</td>
      <td>8062</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2487200875</td>
      <td>20141209T000000</td>
      <td>604000.0</td>
      <td>4</td>
      <td>3.00</td>
      <td>1960</td>
      <td>5000</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1050</td>
      <td>910</td>
      <td>1965</td>
      <td>0</td>
      <td>98136</td>
      <td>47.5208</td>
      <td>-122.393</td>
      <td>1360</td>
      <td>5000</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1954400510</td>
      <td>20150218T000000</td>
      <td>510000.0</td>
      <td>3</td>
      <td>2.00</td>
      <td>1680</td>
      <td>8080</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1680</td>
      <td>0</td>
      <td>1987</td>
      <td>0</td>
      <td>98074</td>
      <td>47.6168</td>
      <td>-122.045</td>
      <td>1800</td>
      <td>7503</td>
    </tr>
  </tbody>
</table>
<p>5 rows × 21 columns</p>
</div>




```python

```


```python

```


```python

```


```python

```


```python
houses
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
      <th>id</th>
      <th>date</th>
      <th>price</th>
      <th>bedrooms</th>
      <th>bathrooms</th>
      <th>sqft_living</th>
      <th>sqft_lot</th>
      <th>floors</th>
      <th>waterfront</th>
      <th>view</th>
      <th>...</th>
      <th>grade</th>
      <th>sqft_above</th>
      <th>sqft_basement</th>
      <th>yr_built</th>
      <th>yr_renovated</th>
      <th>zipcode</th>
      <th>lat</th>
      <th>long</th>
      <th>sqft_living15</th>
      <th>sqft_lot15</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>7129300520</td>
      <td>20141013T000000</td>
      <td>221900.0</td>
      <td>3</td>
      <td>1.00</td>
      <td>1180</td>
      <td>5650</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1180</td>
      <td>0</td>
      <td>1955</td>
      <td>0</td>
      <td>98178</td>
      <td>47.5112</td>
      <td>-122.257</td>
      <td>1340</td>
      <td>5650</td>
    </tr>
    <tr>
      <th>1</th>
      <td>6414100192</td>
      <td>20141209T000000</td>
      <td>538000.0</td>
      <td>3</td>
      <td>2.25</td>
      <td>2570</td>
      <td>7242</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>2170</td>
      <td>400</td>
      <td>1951</td>
      <td>1991</td>
      <td>98125</td>
      <td>47.7210</td>
      <td>-122.319</td>
      <td>1690</td>
      <td>7639</td>
    </tr>
    <tr>
      <th>2</th>
      <td>5631500400</td>
      <td>20150225T000000</td>
      <td>180000.0</td>
      <td>2</td>
      <td>1.00</td>
      <td>770</td>
      <td>10000</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>6</td>
      <td>770</td>
      <td>0</td>
      <td>1933</td>
      <td>0</td>
      <td>98028</td>
      <td>47.7379</td>
      <td>-122.233</td>
      <td>2720</td>
      <td>8062</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2487200875</td>
      <td>20141209T000000</td>
      <td>604000.0</td>
      <td>4</td>
      <td>3.00</td>
      <td>1960</td>
      <td>5000</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1050</td>
      <td>910</td>
      <td>1965</td>
      <td>0</td>
      <td>98136</td>
      <td>47.5208</td>
      <td>-122.393</td>
      <td>1360</td>
      <td>5000</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1954400510</td>
      <td>20150218T000000</td>
      <td>510000.0</td>
      <td>3</td>
      <td>2.00</td>
      <td>1680</td>
      <td>8080</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1680</td>
      <td>0</td>
      <td>1987</td>
      <td>0</td>
      <td>98074</td>
      <td>47.6168</td>
      <td>-122.045</td>
      <td>1800</td>
      <td>7503</td>
    </tr>
    <tr>
      <th>5</th>
      <td>7237550310</td>
      <td>20140512T000000</td>
      <td>1225000.0</td>
      <td>4</td>
      <td>4.50</td>
      <td>5420</td>
      <td>101930</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>11</td>
      <td>3890</td>
      <td>1530</td>
      <td>2001</td>
      <td>0</td>
      <td>98053</td>
      <td>47.6561</td>
      <td>-122.005</td>
      <td>4760</td>
      <td>101930</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1321400060</td>
      <td>20140627T000000</td>
      <td>257500.0</td>
      <td>3</td>
      <td>2.25</td>
      <td>1715</td>
      <td>6819</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1715</td>
      <td>0</td>
      <td>1995</td>
      <td>0</td>
      <td>98003</td>
      <td>47.3097</td>
      <td>-122.327</td>
      <td>2238</td>
      <td>6819</td>
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
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>21606</th>
      <td>7936000429</td>
      <td>20150326T000000</td>
      <td>1007500.0</td>
      <td>4</td>
      <td>3.50</td>
      <td>3510</td>
      <td>7200</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>9</td>
      <td>2600</td>
      <td>910</td>
      <td>2009</td>
      <td>0</td>
      <td>98136</td>
      <td>47.5537</td>
      <td>-122.398</td>
      <td>2050</td>
      <td>6200</td>
    </tr>
    <tr>
      <th>21607</th>
      <td>2997800021</td>
      <td>20150219T000000</td>
      <td>475000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1310</td>
      <td>1294</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1180</td>
      <td>130</td>
      <td>2008</td>
      <td>0</td>
      <td>98116</td>
      <td>47.5773</td>
      <td>-122.409</td>
      <td>1330</td>
      <td>1265</td>
    </tr>
    <tr>
      <th>21608</th>
      <td>263000018</td>
      <td>20140521T000000</td>
      <td>360000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1530</td>
      <td>1131</td>
      <td>3.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1530</td>
      <td>0</td>
      <td>2009</td>
      <td>0</td>
      <td>98103</td>
      <td>47.6993</td>
      <td>-122.346</td>
      <td>1530</td>
      <td>1509</td>
    </tr>
    <tr>
      <th>21609</th>
      <td>6600060120</td>
      <td>20150223T000000</td>
      <td>400000.0</td>
      <td>4</td>
      <td>2.50</td>
      <td>2310</td>
      <td>5813</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>2310</td>
      <td>0</td>
      <td>2014</td>
      <td>0</td>
      <td>98146</td>
      <td>47.5107</td>
      <td>-122.362</td>
      <td>1830</td>
      <td>7200</td>
    </tr>
    <tr>
      <th>21610</th>
      <td>1523300141</td>
      <td>20140623T000000</td>
      <td>402101.0</td>
      <td>2</td>
      <td>0.75</td>
      <td>1020</td>
      <td>1350</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1020</td>
      <td>0</td>
      <td>2009</td>
      <td>0</td>
      <td>98144</td>
      <td>47.5944</td>
      <td>-122.299</td>
      <td>1020</td>
      <td>2007</td>
    </tr>
    <tr>
      <th>21611</th>
      <td>291310100</td>
      <td>20150116T000000</td>
      <td>400000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1600</td>
      <td>2388</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1600</td>
      <td>0</td>
      <td>2004</td>
      <td>0</td>
      <td>98027</td>
      <td>47.5345</td>
      <td>-122.069</td>
      <td>1410</td>
      <td>1287</td>
    </tr>
    <tr>
      <th>21612</th>
      <td>1523300157</td>
      <td>20141015T000000</td>
      <td>325000.0</td>
      <td>2</td>
      <td>0.75</td>
      <td>1020</td>
      <td>1076</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1020</td>
      <td>0</td>
      <td>2008</td>
      <td>0</td>
      <td>98144</td>
      <td>47.5941</td>
      <td>-122.299</td>
      <td>1020</td>
      <td>1357</td>
    </tr>
  </tbody>
</table>
<p>21613 rows × 21 columns</p>
</div>




```python
type(houses)
```




    pandas.core.frame.DataFrame




```python
houses.columns
```




    Index(['id', 'date', 'price', 'bedrooms', 'bathrooms', 'sqft_living',
           'sqft_lot', 'floors', 'waterfront', 'view', 'condition', 'grade',
           'sqft_above', 'sqft_basement', 'yr_built', 'yr_renovated', 'zipcode',
           'lat', 'long', 'sqft_living15', 'sqft_lot15'],
          dtype='object')




```python
states.columns
```




    Index(['State', 'Abbrev', 'Code'], dtype='object')




```python
len(houses)
```




    21613




```python
houses.shape
```




    (21613, 21)




```python
houses.size
```




    453873




```python
pd.options.display.min_rows = 15
```


```python
houses
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
      <th>id</th>
      <th>date</th>
      <th>price</th>
      <th>bedrooms</th>
      <th>bathrooms</th>
      <th>sqft_living</th>
      <th>sqft_lot</th>
      <th>floors</th>
      <th>waterfront</th>
      <th>view</th>
      <th>...</th>
      <th>grade</th>
      <th>sqft_above</th>
      <th>sqft_basement</th>
      <th>yr_built</th>
      <th>yr_renovated</th>
      <th>zipcode</th>
      <th>lat</th>
      <th>long</th>
      <th>sqft_living15</th>
      <th>sqft_lot15</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>7129300520</td>
      <td>20141013T000000</td>
      <td>221900.0</td>
      <td>3</td>
      <td>1.00</td>
      <td>1180</td>
      <td>5650</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1180</td>
      <td>0</td>
      <td>1955</td>
      <td>0</td>
      <td>98178</td>
      <td>47.5112</td>
      <td>-122.257</td>
      <td>1340</td>
      <td>5650</td>
    </tr>
    <tr>
      <th>1</th>
      <td>6414100192</td>
      <td>20141209T000000</td>
      <td>538000.0</td>
      <td>3</td>
      <td>2.25</td>
      <td>2570</td>
      <td>7242</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>2170</td>
      <td>400</td>
      <td>1951</td>
      <td>1991</td>
      <td>98125</td>
      <td>47.7210</td>
      <td>-122.319</td>
      <td>1690</td>
      <td>7639</td>
    </tr>
    <tr>
      <th>2</th>
      <td>5631500400</td>
      <td>20150225T000000</td>
      <td>180000.0</td>
      <td>2</td>
      <td>1.00</td>
      <td>770</td>
      <td>10000</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>6</td>
      <td>770</td>
      <td>0</td>
      <td>1933</td>
      <td>0</td>
      <td>98028</td>
      <td>47.7379</td>
      <td>-122.233</td>
      <td>2720</td>
      <td>8062</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2487200875</td>
      <td>20141209T000000</td>
      <td>604000.0</td>
      <td>4</td>
      <td>3.00</td>
      <td>1960</td>
      <td>5000</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1050</td>
      <td>910</td>
      <td>1965</td>
      <td>0</td>
      <td>98136</td>
      <td>47.5208</td>
      <td>-122.393</td>
      <td>1360</td>
      <td>5000</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1954400510</td>
      <td>20150218T000000</td>
      <td>510000.0</td>
      <td>3</td>
      <td>2.00</td>
      <td>1680</td>
      <td>8080</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1680</td>
      <td>0</td>
      <td>1987</td>
      <td>0</td>
      <td>98074</td>
      <td>47.6168</td>
      <td>-122.045</td>
      <td>1800</td>
      <td>7503</td>
    </tr>
    <tr>
      <th>5</th>
      <td>7237550310</td>
      <td>20140512T000000</td>
      <td>1225000.0</td>
      <td>4</td>
      <td>4.50</td>
      <td>5420</td>
      <td>101930</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>11</td>
      <td>3890</td>
      <td>1530</td>
      <td>2001</td>
      <td>0</td>
      <td>98053</td>
      <td>47.6561</td>
      <td>-122.005</td>
      <td>4760</td>
      <td>101930</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1321400060</td>
      <td>20140627T000000</td>
      <td>257500.0</td>
      <td>3</td>
      <td>2.25</td>
      <td>1715</td>
      <td>6819</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1715</td>
      <td>0</td>
      <td>1995</td>
      <td>0</td>
      <td>98003</td>
      <td>47.3097</td>
      <td>-122.327</td>
      <td>2238</td>
      <td>6819</td>
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
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>21606</th>
      <td>7936000429</td>
      <td>20150326T000000</td>
      <td>1007500.0</td>
      <td>4</td>
      <td>3.50</td>
      <td>3510</td>
      <td>7200</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>9</td>
      <td>2600</td>
      <td>910</td>
      <td>2009</td>
      <td>0</td>
      <td>98136</td>
      <td>47.5537</td>
      <td>-122.398</td>
      <td>2050</td>
      <td>6200</td>
    </tr>
    <tr>
      <th>21607</th>
      <td>2997800021</td>
      <td>20150219T000000</td>
      <td>475000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1310</td>
      <td>1294</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1180</td>
      <td>130</td>
      <td>2008</td>
      <td>0</td>
      <td>98116</td>
      <td>47.5773</td>
      <td>-122.409</td>
      <td>1330</td>
      <td>1265</td>
    </tr>
    <tr>
      <th>21608</th>
      <td>263000018</td>
      <td>20140521T000000</td>
      <td>360000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1530</td>
      <td>1131</td>
      <td>3.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1530</td>
      <td>0</td>
      <td>2009</td>
      <td>0</td>
      <td>98103</td>
      <td>47.6993</td>
      <td>-122.346</td>
      <td>1530</td>
      <td>1509</td>
    </tr>
    <tr>
      <th>21609</th>
      <td>6600060120</td>
      <td>20150223T000000</td>
      <td>400000.0</td>
      <td>4</td>
      <td>2.50</td>
      <td>2310</td>
      <td>5813</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>2310</td>
      <td>0</td>
      <td>2014</td>
      <td>0</td>
      <td>98146</td>
      <td>47.5107</td>
      <td>-122.362</td>
      <td>1830</td>
      <td>7200</td>
    </tr>
    <tr>
      <th>21610</th>
      <td>1523300141</td>
      <td>20140623T000000</td>
      <td>402101.0</td>
      <td>2</td>
      <td>0.75</td>
      <td>1020</td>
      <td>1350</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1020</td>
      <td>0</td>
      <td>2009</td>
      <td>0</td>
      <td>98144</td>
      <td>47.5944</td>
      <td>-122.299</td>
      <td>1020</td>
      <td>2007</td>
    </tr>
    <tr>
      <th>21611</th>
      <td>291310100</td>
      <td>20150116T000000</td>
      <td>400000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1600</td>
      <td>2388</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1600</td>
      <td>0</td>
      <td>2004</td>
      <td>0</td>
      <td>98027</td>
      <td>47.5345</td>
      <td>-122.069</td>
      <td>1410</td>
      <td>1287</td>
    </tr>
    <tr>
      <th>21612</th>
      <td>1523300157</td>
      <td>20141015T000000</td>
      <td>325000.0</td>
      <td>2</td>
      <td>0.75</td>
      <td>1020</td>
      <td>1076</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1020</td>
      <td>0</td>
      <td>2008</td>
      <td>0</td>
      <td>98144</td>
      <td>47.5941</td>
      <td>-122.299</td>
      <td>1020</td>
      <td>1357</td>
    </tr>
  </tbody>
</table>
<p>21613 rows × 21 columns</p>
</div>



The `head()` method returns the first n rows in a NEW DataFrame


```python
first_5 = houses.head()
first_5
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
      <th>id</th>
      <th>date</th>
      <th>price</th>
      <th>bedrooms</th>
      <th>bathrooms</th>
      <th>sqft_living</th>
      <th>sqft_lot</th>
      <th>floors</th>
      <th>waterfront</th>
      <th>view</th>
      <th>...</th>
      <th>grade</th>
      <th>sqft_above</th>
      <th>sqft_basement</th>
      <th>yr_built</th>
      <th>yr_renovated</th>
      <th>zipcode</th>
      <th>lat</th>
      <th>long</th>
      <th>sqft_living15</th>
      <th>sqft_lot15</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>7129300520</td>
      <td>20141013T000000</td>
      <td>221900.0</td>
      <td>3</td>
      <td>1.00</td>
      <td>1180</td>
      <td>5650</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1180</td>
      <td>0</td>
      <td>1955</td>
      <td>0</td>
      <td>98178</td>
      <td>47.5112</td>
      <td>-122.257</td>
      <td>1340</td>
      <td>5650</td>
    </tr>
    <tr>
      <th>1</th>
      <td>6414100192</td>
      <td>20141209T000000</td>
      <td>538000.0</td>
      <td>3</td>
      <td>2.25</td>
      <td>2570</td>
      <td>7242</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>2170</td>
      <td>400</td>
      <td>1951</td>
      <td>1991</td>
      <td>98125</td>
      <td>47.7210</td>
      <td>-122.319</td>
      <td>1690</td>
      <td>7639</td>
    </tr>
    <tr>
      <th>2</th>
      <td>5631500400</td>
      <td>20150225T000000</td>
      <td>180000.0</td>
      <td>2</td>
      <td>1.00</td>
      <td>770</td>
      <td>10000</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>6</td>
      <td>770</td>
      <td>0</td>
      <td>1933</td>
      <td>0</td>
      <td>98028</td>
      <td>47.7379</td>
      <td>-122.233</td>
      <td>2720</td>
      <td>8062</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2487200875</td>
      <td>20141209T000000</td>
      <td>604000.0</td>
      <td>4</td>
      <td>3.00</td>
      <td>1960</td>
      <td>5000</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1050</td>
      <td>910</td>
      <td>1965</td>
      <td>0</td>
      <td>98136</td>
      <td>47.5208</td>
      <td>-122.393</td>
      <td>1360</td>
      <td>5000</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1954400510</td>
      <td>20150218T000000</td>
      <td>510000.0</td>
      <td>3</td>
      <td>2.00</td>
      <td>1680</td>
      <td>8080</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1680</td>
      <td>0</td>
      <td>1987</td>
      <td>0</td>
      <td>98074</td>
      <td>47.6168</td>
      <td>-122.045</td>
      <td>1800</td>
      <td>7503</td>
    </tr>
  </tbody>
</table>
<p>5 rows × 21 columns</p>
</div>




```python
type(first_5)
```




    pandas.core.frame.DataFrame




```python
houses.head(200)
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
      <th>id</th>
      <th>date</th>
      <th>price</th>
      <th>bedrooms</th>
      <th>bathrooms</th>
      <th>sqft_living</th>
      <th>sqft_lot</th>
      <th>floors</th>
      <th>waterfront</th>
      <th>view</th>
      <th>...</th>
      <th>grade</th>
      <th>sqft_above</th>
      <th>sqft_basement</th>
      <th>yr_built</th>
      <th>yr_renovated</th>
      <th>zipcode</th>
      <th>lat</th>
      <th>long</th>
      <th>sqft_living15</th>
      <th>sqft_lot15</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>7129300520</td>
      <td>20141013T000000</td>
      <td>221900.0</td>
      <td>3</td>
      <td>1.00</td>
      <td>1180</td>
      <td>5650</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1180</td>
      <td>0</td>
      <td>1955</td>
      <td>0</td>
      <td>98178</td>
      <td>47.5112</td>
      <td>-122.257</td>
      <td>1340</td>
      <td>5650</td>
    </tr>
    <tr>
      <th>1</th>
      <td>6414100192</td>
      <td>20141209T000000</td>
      <td>538000.0</td>
      <td>3</td>
      <td>2.25</td>
      <td>2570</td>
      <td>7242</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>2170</td>
      <td>400</td>
      <td>1951</td>
      <td>1991</td>
      <td>98125</td>
      <td>47.7210</td>
      <td>-122.319</td>
      <td>1690</td>
      <td>7639</td>
    </tr>
    <tr>
      <th>2</th>
      <td>5631500400</td>
      <td>20150225T000000</td>
      <td>180000.0</td>
      <td>2</td>
      <td>1.00</td>
      <td>770</td>
      <td>10000</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>6</td>
      <td>770</td>
      <td>0</td>
      <td>1933</td>
      <td>0</td>
      <td>98028</td>
      <td>47.7379</td>
      <td>-122.233</td>
      <td>2720</td>
      <td>8062</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2487200875</td>
      <td>20141209T000000</td>
      <td>604000.0</td>
      <td>4</td>
      <td>3.00</td>
      <td>1960</td>
      <td>5000</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1050</td>
      <td>910</td>
      <td>1965</td>
      <td>0</td>
      <td>98136</td>
      <td>47.5208</td>
      <td>-122.393</td>
      <td>1360</td>
      <td>5000</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1954400510</td>
      <td>20150218T000000</td>
      <td>510000.0</td>
      <td>3</td>
      <td>2.00</td>
      <td>1680</td>
      <td>8080</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1680</td>
      <td>0</td>
      <td>1987</td>
      <td>0</td>
      <td>98074</td>
      <td>47.6168</td>
      <td>-122.045</td>
      <td>1800</td>
      <td>7503</td>
    </tr>
    <tr>
      <th>5</th>
      <td>7237550310</td>
      <td>20140512T000000</td>
      <td>1225000.0</td>
      <td>4</td>
      <td>4.50</td>
      <td>5420</td>
      <td>101930</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>11</td>
      <td>3890</td>
      <td>1530</td>
      <td>2001</td>
      <td>0</td>
      <td>98053</td>
      <td>47.6561</td>
      <td>-122.005</td>
      <td>4760</td>
      <td>101930</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1321400060</td>
      <td>20140627T000000</td>
      <td>257500.0</td>
      <td>3</td>
      <td>2.25</td>
      <td>1715</td>
      <td>6819</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1715</td>
      <td>0</td>
      <td>1995</td>
      <td>0</td>
      <td>98003</td>
      <td>47.3097</td>
      <td>-122.327</td>
      <td>2238</td>
      <td>6819</td>
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
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>193</th>
      <td>3663500060</td>
      <td>20140625T000000</td>
      <td>400000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>2180</td>
      <td>7508</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1420</td>
      <td>760</td>
      <td>1962</td>
      <td>0</td>
      <td>98133</td>
      <td>47.7606</td>
      <td>-122.336</td>
      <td>1900</td>
      <td>7818</td>
    </tr>
    <tr>
      <th>194</th>
      <td>3996900125</td>
      <td>20141201T000000</td>
      <td>230000.0</td>
      <td>3</td>
      <td>1.00</td>
      <td>1060</td>
      <td>10228</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1060</td>
      <td>0</td>
      <td>1948</td>
      <td>0</td>
      <td>98155</td>
      <td>47.7481</td>
      <td>-122.300</td>
      <td>1570</td>
      <td>10228</td>
    </tr>
    <tr>
      <th>195</th>
      <td>7796450200</td>
      <td>20140515T000000</td>
      <td>256883.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1690</td>
      <td>5025</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1690</td>
      <td>0</td>
      <td>2003</td>
      <td>0</td>
      <td>98023</td>
      <td>47.2779</td>
      <td>-122.347</td>
      <td>2550</td>
      <td>5001</td>
    </tr>
    <tr>
      <th>196</th>
      <td>7549802535</td>
      <td>20141111T000000</td>
      <td>423000.0</td>
      <td>4</td>
      <td>2.00</td>
      <td>1970</td>
      <td>6480</td>
      <td>1.5</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1130</td>
      <td>840</td>
      <td>1920</td>
      <td>0</td>
      <td>98108</td>
      <td>47.5511</td>
      <td>-122.312</td>
      <td>1500</td>
      <td>6480</td>
    </tr>
    <tr>
      <th>197</th>
      <td>3278600320</td>
      <td>20140723T000000</td>
      <td>465000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>2150</td>
      <td>4084</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>2150</td>
      <td>0</td>
      <td>2007</td>
      <td>0</td>
      <td>98126</td>
      <td>47.5488</td>
      <td>-122.372</td>
      <td>1750</td>
      <td>2385</td>
    </tr>
    <tr>
      <th>198</th>
      <td>2824079053</td>
      <td>20150113T000000</td>
      <td>440000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1910</td>
      <td>66211</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1910</td>
      <td>0</td>
      <td>1997</td>
      <td>0</td>
      <td>98024</td>
      <td>47.5385</td>
      <td>-121.911</td>
      <td>2330</td>
      <td>67268</td>
    </tr>
    <tr>
      <th>199</th>
      <td>1222069094</td>
      <td>20141014T000000</td>
      <td>385000.0</td>
      <td>3</td>
      <td>1.75</td>
      <td>1350</td>
      <td>155073</td>
      <td>1.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1350</td>
      <td>0</td>
      <td>1969</td>
      <td>0</td>
      <td>98038</td>
      <td>47.4058</td>
      <td>-121.994</td>
      <td>1560</td>
      <td>50965</td>
    </tr>
  </tbody>
</table>
<p>200 rows × 21 columns</p>
</div>



The `tail()` method is like `head()` but it works from the END of a DataFrame.  By default it returns the last 5 rows in a new DataFrame.


```python
houses.tail()
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
      <th>id</th>
      <th>date</th>
      <th>price</th>
      <th>bedrooms</th>
      <th>bathrooms</th>
      <th>sqft_living</th>
      <th>sqft_lot</th>
      <th>floors</th>
      <th>waterfront</th>
      <th>view</th>
      <th>...</th>
      <th>grade</th>
      <th>sqft_above</th>
      <th>sqft_basement</th>
      <th>yr_built</th>
      <th>yr_renovated</th>
      <th>zipcode</th>
      <th>lat</th>
      <th>long</th>
      <th>sqft_living15</th>
      <th>sqft_lot15</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>21608</th>
      <td>263000018</td>
      <td>20140521T000000</td>
      <td>360000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1530</td>
      <td>1131</td>
      <td>3.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1530</td>
      <td>0</td>
      <td>2009</td>
      <td>0</td>
      <td>98103</td>
      <td>47.6993</td>
      <td>-122.346</td>
      <td>1530</td>
      <td>1509</td>
    </tr>
    <tr>
      <th>21609</th>
      <td>6600060120</td>
      <td>20150223T000000</td>
      <td>400000.0</td>
      <td>4</td>
      <td>2.50</td>
      <td>2310</td>
      <td>5813</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>2310</td>
      <td>0</td>
      <td>2014</td>
      <td>0</td>
      <td>98146</td>
      <td>47.5107</td>
      <td>-122.362</td>
      <td>1830</td>
      <td>7200</td>
    </tr>
    <tr>
      <th>21610</th>
      <td>1523300141</td>
      <td>20140623T000000</td>
      <td>402101.0</td>
      <td>2</td>
      <td>0.75</td>
      <td>1020</td>
      <td>1350</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1020</td>
      <td>0</td>
      <td>2009</td>
      <td>0</td>
      <td>98144</td>
      <td>47.5944</td>
      <td>-122.299</td>
      <td>1020</td>
      <td>2007</td>
    </tr>
    <tr>
      <th>21611</th>
      <td>291310100</td>
      <td>20150116T000000</td>
      <td>400000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1600</td>
      <td>2388</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1600</td>
      <td>0</td>
      <td>2004</td>
      <td>0</td>
      <td>98027</td>
      <td>47.5345</td>
      <td>-122.069</td>
      <td>1410</td>
      <td>1287</td>
    </tr>
    <tr>
      <th>21612</th>
      <td>1523300157</td>
      <td>20141015T000000</td>
      <td>325000.0</td>
      <td>2</td>
      <td>0.75</td>
      <td>1020</td>
      <td>1076</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1020</td>
      <td>0</td>
      <td>2008</td>
      <td>0</td>
      <td>98144</td>
      <td>47.5941</td>
      <td>-122.299</td>
      <td>1020</td>
      <td>1357</td>
    </tr>
  </tbody>
</table>
<p>5 rows × 21 columns</p>
</div>




```python
houses.tail(9)
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
      <th>id</th>
      <th>date</th>
      <th>price</th>
      <th>bedrooms</th>
      <th>bathrooms</th>
      <th>sqft_living</th>
      <th>sqft_lot</th>
      <th>floors</th>
      <th>waterfront</th>
      <th>view</th>
      <th>...</th>
      <th>grade</th>
      <th>sqft_above</th>
      <th>sqft_basement</th>
      <th>yr_built</th>
      <th>yr_renovated</th>
      <th>zipcode</th>
      <th>lat</th>
      <th>long</th>
      <th>sqft_living15</th>
      <th>sqft_lot15</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>21604</th>
      <td>9834201367</td>
      <td>20150126T000000</td>
      <td>429000.0</td>
      <td>3</td>
      <td>2.00</td>
      <td>1490</td>
      <td>1126</td>
      <td>3.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1490</td>
      <td>0</td>
      <td>2014</td>
      <td>0</td>
      <td>98144</td>
      <td>47.5699</td>
      <td>-122.288</td>
      <td>1400</td>
      <td>1230</td>
    </tr>
    <tr>
      <th>21605</th>
      <td>3448900210</td>
      <td>20141014T000000</td>
      <td>610685.0</td>
      <td>4</td>
      <td>2.50</td>
      <td>2520</td>
      <td>6023</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>9</td>
      <td>2520</td>
      <td>0</td>
      <td>2014</td>
      <td>0</td>
      <td>98056</td>
      <td>47.5137</td>
      <td>-122.167</td>
      <td>2520</td>
      <td>6023</td>
    </tr>
    <tr>
      <th>21606</th>
      <td>7936000429</td>
      <td>20150326T000000</td>
      <td>1007500.0</td>
      <td>4</td>
      <td>3.50</td>
      <td>3510</td>
      <td>7200</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>9</td>
      <td>2600</td>
      <td>910</td>
      <td>2009</td>
      <td>0</td>
      <td>98136</td>
      <td>47.5537</td>
      <td>-122.398</td>
      <td>2050</td>
      <td>6200</td>
    </tr>
    <tr>
      <th>21607</th>
      <td>2997800021</td>
      <td>20150219T000000</td>
      <td>475000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1310</td>
      <td>1294</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1180</td>
      <td>130</td>
      <td>2008</td>
      <td>0</td>
      <td>98116</td>
      <td>47.5773</td>
      <td>-122.409</td>
      <td>1330</td>
      <td>1265</td>
    </tr>
    <tr>
      <th>21608</th>
      <td>263000018</td>
      <td>20140521T000000</td>
      <td>360000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1530</td>
      <td>1131</td>
      <td>3.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1530</td>
      <td>0</td>
      <td>2009</td>
      <td>0</td>
      <td>98103</td>
      <td>47.6993</td>
      <td>-122.346</td>
      <td>1530</td>
      <td>1509</td>
    </tr>
    <tr>
      <th>21609</th>
      <td>6600060120</td>
      <td>20150223T000000</td>
      <td>400000.0</td>
      <td>4</td>
      <td>2.50</td>
      <td>2310</td>
      <td>5813</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>2310</td>
      <td>0</td>
      <td>2014</td>
      <td>0</td>
      <td>98146</td>
      <td>47.5107</td>
      <td>-122.362</td>
      <td>1830</td>
      <td>7200</td>
    </tr>
    <tr>
      <th>21610</th>
      <td>1523300141</td>
      <td>20140623T000000</td>
      <td>402101.0</td>
      <td>2</td>
      <td>0.75</td>
      <td>1020</td>
      <td>1350</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1020</td>
      <td>0</td>
      <td>2009</td>
      <td>0</td>
      <td>98144</td>
      <td>47.5944</td>
      <td>-122.299</td>
      <td>1020</td>
      <td>2007</td>
    </tr>
    <tr>
      <th>21611</th>
      <td>291310100</td>
      <td>20150116T000000</td>
      <td>400000.0</td>
      <td>3</td>
      <td>2.50</td>
      <td>1600</td>
      <td>2388</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>8</td>
      <td>1600</td>
      <td>0</td>
      <td>2004</td>
      <td>0</td>
      <td>98027</td>
      <td>47.5345</td>
      <td>-122.069</td>
      <td>1410</td>
      <td>1287</td>
    </tr>
    <tr>
      <th>21612</th>
      <td>1523300157</td>
      <td>20141015T000000</td>
      <td>325000.0</td>
      <td>2</td>
      <td>0.75</td>
      <td>1020</td>
      <td>1076</td>
      <td>2.0</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>7</td>
      <td>1020</td>
      <td>0</td>
      <td>2008</td>
      <td>0</td>
      <td>98144</td>
      <td>47.5941</td>
      <td>-122.299</td>
      <td>1020</td>
      <td>1357</td>
    </tr>
  </tbody>
</table>
<p>9 rows × 21 columns</p>
</div>




```python
houses.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 21613 entries, 0 to 21612
    Data columns (total 21 columns):
     #   Column         Non-Null Count  Dtype  
    ---  ------         --------------  -----  
     0   id             21613 non-null  int64  
     1   date           21613 non-null  object 
     2   price          21613 non-null  float64
     3   bedrooms       21613 non-null  int64  
     4   bathrooms      21613 non-null  float64
     5   sqft_living    21613 non-null  int64  
     6   sqft_lot       21613 non-null  int64  
     7   floors         21613 non-null  float64
     8   waterfront     21613 non-null  int64  
     9   view           21613 non-null  int64  
     10  condition      21613 non-null  int64  
     11  grade          21613 non-null  int64  
     12  sqft_above     21613 non-null  int64  
     13  sqft_basement  21613 non-null  int64  
     14  yr_built       21613 non-null  int64  
     15  yr_renovated   21613 non-null  int64  
     16  zipcode        21613 non-null  int64  
     17  lat            21613 non-null  float64
     18  long           21613 non-null  float64
     19  sqft_living15  21613 non-null  int64  
     20  sqft_lot15     21613 non-null  int64  
    dtypes: float64(5), int64(15), object(1)
    memory usage: 3.5+ MB
    


```python
states.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 51 entries, 0 to 50
    Data columns (total 3 columns):
     #   Column  Non-Null Count  Dtype 
    ---  ------  --------------  ----- 
     0   State   51 non-null     object
     1   Abbrev  51 non-null     object
     2   Code    51 non-null     object
    dtypes: object(3)
    memory usage: 1.3+ KB
    


```python
houses.dtypes
```




    id                 int64
    date              object
    price            float64
    bedrooms           int64
    bathrooms        float64
    sqft_living        int64
    sqft_lot           int64
    floors           float64
    waterfront         int64
    view               int64
    condition          int64
    grade              int64
    sqft_above         int64
    sqft_basement      int64
    yr_built           int64
    yr_renovated       int64
    zipcode            int64
    lat              float64
    long             float64
    sqft_living15      int64
    sqft_lot15         int64
    dtype: object



## Introducing The Titanic Dataset


```python
titanic = pd.read_csv("data/titanic.csv")
titanic.head()
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
      <th>pclass</th>
      <th>survived</th>
      <th>name</th>
      <th>sex</th>
      <th>age</th>
      <th>sibsp</th>
      <th>parch</th>
      <th>ticket</th>
      <th>fare</th>
      <th>cabin</th>
      <th>embarked</th>
      <th>boat</th>
      <th>body</th>
      <th>home.dest</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>1</td>
      <td>Allen, Miss. Elisabeth Walton</td>
      <td>female</td>
      <td>29</td>
      <td>0</td>
      <td>0</td>
      <td>24160</td>
      <td>211.3375</td>
      <td>B5</td>
      <td>S</td>
      <td>2</td>
      <td>?</td>
      <td>St Louis, MO</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>1</td>
      <td>Allison, Master. Hudson Trevor</td>
      <td>male</td>
      <td>0.9167</td>
      <td>1</td>
      <td>2</td>
      <td>113781</td>
      <td>151.55</td>
      <td>C22 C26</td>
      <td>S</td>
      <td>11</td>
      <td>?</td>
      <td>Montreal, PQ / Chesterville, ON</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1</td>
      <td>0</td>
      <td>Allison, Miss. Helen Loraine</td>
      <td>female</td>
      <td>2</td>
      <td>1</td>
      <td>2</td>
      <td>113781</td>
      <td>151.55</td>
      <td>C22 C26</td>
      <td>S</td>
      <td>?</td>
      <td>?</td>
      <td>Montreal, PQ / Chesterville, ON</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1</td>
      <td>0</td>
      <td>Allison, Mr. Hudson Joshua Creighton</td>
      <td>male</td>
      <td>30</td>
      <td>1</td>
      <td>2</td>
      <td>113781</td>
      <td>151.55</td>
      <td>C22 C26</td>
      <td>S</td>
      <td>?</td>
      <td>135</td>
      <td>Montreal, PQ / Chesterville, ON</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1</td>
      <td>0</td>
      <td>Allison, Mrs. Hudson J C (Bessie Waldo Daniels)</td>
      <td>female</td>
      <td>25</td>
      <td>1</td>
      <td>2</td>
      <td>113781</td>
      <td>151.55</td>
      <td>C22 C26</td>
      <td>S</td>
      <td>?</td>
      <td>?</td>
      <td>Montreal, PQ / Chesterville, ON</td>
    </tr>
  </tbody>
</table>
</div>




```python
titanic.columns
```




    Index(['pclass', 'survived', 'name', 'sex', 'age', 'sibsp', 'parch', 'ticket',
           'fare', 'cabin', 'embarked', 'boat', 'body', 'home.dest'],
          dtype='object')



* `pclass` - Passenger Class (1 = 1st; 2 = 2nd; 3 = 3rd)
* `survived` - Survival (0 = No; 1 = Yes)
* `name` - Name
* `sex` - Sex
* `age` - Age
* `sibsp` - Number of Siblings/Spouses Aboard
* `parch` - Number of Parents/Children Aboard
* `ticket` - Ticket Number
* `fare` - Passenger Fare
* `cabin` - Cabin
* `embarked` - Port of Embarkation (C = Cherbourg; Q = Queenstown; S = Southampton)
* `boat` - Lifeboat (if survived)
* `body` - Body number (if did not survive and body was recovered)
* `home.dest` - Home/Destination


```python
titanic.tail(10)
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
      <th>pclass</th>
      <th>survived</th>
      <th>name</th>
      <th>sex</th>
      <th>age</th>
      <th>sibsp</th>
      <th>parch</th>
      <th>ticket</th>
      <th>fare</th>
      <th>cabin</th>
      <th>embarked</th>
      <th>boat</th>
      <th>body</th>
      <th>home.dest</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1299</th>
      <td>3</td>
      <td>0</td>
      <td>Yasbeck, Mr. Antoni</td>
      <td>male</td>
      <td>27</td>
      <td>1</td>
      <td>0</td>
      <td>2659</td>
      <td>14.4542</td>
      <td>?</td>
      <td>C</td>
      <td>C</td>
      <td>?</td>
      <td>?</td>
    </tr>
    <tr>
      <th>1300</th>
      <td>3</td>
      <td>1</td>
      <td>Yasbeck, Mrs. Antoni (Selini Alexander)</td>
      <td>female</td>
      <td>15</td>
      <td>1</td>
      <td>0</td>
      <td>2659</td>
      <td>14.4542</td>
      <td>?</td>
      <td>C</td>
      <td>?</td>
      <td>?</td>
      <td>?</td>
    </tr>
    <tr>
      <th>1301</th>
      <td>3</td>
      <td>0</td>
      <td>Youseff, Mr. Gerious</td>
      <td>male</td>
      <td>45.5</td>
      <td>0</td>
      <td>0</td>
      <td>2628</td>
      <td>7.225</td>
      <td>?</td>
      <td>C</td>
      <td>?</td>
      <td>312</td>
      <td>?</td>
    </tr>
    <tr>
      <th>1302</th>
      <td>3</td>
      <td>0</td>
      <td>Yousif, Mr. Wazli</td>
      <td>male</td>
      <td>?</td>
      <td>0</td>
      <td>0</td>
      <td>2647</td>
      <td>7.225</td>
      <td>?</td>
      <td>C</td>
      <td>?</td>
      <td>?</td>
      <td>?</td>
    </tr>
    <tr>
      <th>1303</th>
      <td>3</td>
      <td>0</td>
      <td>Yousseff, Mr. Gerious</td>
      <td>male</td>
      <td>?</td>
      <td>0</td>
      <td>0</td>
      <td>2627</td>
      <td>14.4583</td>
      <td>?</td>
      <td>C</td>
      <td>?</td>
      <td>?</td>
      <td>?</td>
    </tr>
    <tr>
      <th>1304</th>
      <td>3</td>
      <td>0</td>
      <td>Zabour, Miss. Hileni</td>
      <td>female</td>
      <td>14.5</td>
      <td>1</td>
      <td>0</td>
      <td>2665</td>
      <td>14.4542</td>
      <td>?</td>
      <td>C</td>
      <td>?</td>
      <td>328</td>
      <td>?</td>
    </tr>
    <tr>
      <th>1305</th>
      <td>3</td>
      <td>0</td>
      <td>Zabour, Miss. Thamine</td>
      <td>female</td>
      <td>?</td>
      <td>1</td>
      <td>0</td>
      <td>2665</td>
      <td>14.4542</td>
      <td>?</td>
      <td>C</td>
      <td>?</td>
      <td>?</td>
      <td>?</td>
    </tr>
    <tr>
      <th>1306</th>
      <td>3</td>
      <td>0</td>
      <td>Zakarian, Mr. Mapriededer</td>
      <td>male</td>
      <td>26.5</td>
      <td>0</td>
      <td>0</td>
      <td>2656</td>
      <td>7.225</td>
      <td>?</td>
      <td>C</td>
      <td>?</td>
      <td>304</td>
      <td>?</td>
    </tr>
    <tr>
      <th>1307</th>
      <td>3</td>
      <td>0</td>
      <td>Zakarian, Mr. Ortin</td>
      <td>male</td>
      <td>27</td>
      <td>0</td>
      <td>0</td>
      <td>2670</td>
      <td>7.225</td>
      <td>?</td>
      <td>C</td>
      <td>?</td>
      <td>?</td>
      <td>?</td>
    </tr>
    <tr>
      <th>1308</th>
      <td>3</td>
      <td>0</td>
      <td>Zimmerman, Mr. Leo</td>
      <td>male</td>
      <td>29</td>
      <td>0</td>
      <td>0</td>
      <td>315082</td>
      <td>7.875</td>
      <td>?</td>
      <td>S</td>
      <td>?</td>
      <td>?</td>
      <td>?</td>
    </tr>
  </tbody>
</table>
</div>




```python
titanic.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 1309 entries, 0 to 1308
    Data columns (total 14 columns):
     #   Column     Non-Null Count  Dtype 
    ---  ------     --------------  ----- 
     0   pclass     1309 non-null   int64 
     1   survived   1309 non-null   int64 
     2   name       1309 non-null   object
     3   sex        1309 non-null   object
     4   age        1309 non-null   object
     5   sibsp      1309 non-null   int64 
     6   parch      1309 non-null   int64 
     7   ticket     1309 non-null   object
     8   fare       1309 non-null   object
     9   cabin      1309 non-null   object
     10  embarked   1309 non-null   object
     11  boat       1309 non-null   object
     12  body       1309 non-null   object
     13  home.dest  1309 non-null   object
    dtypes: int64(4), object(10)
    memory usage: 143.3+ KB
    


```python
titanic.head()
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
      <th>pclass</th>
      <th>survived</th>
      <th>name</th>
      <th>sex</th>
      <th>age</th>
      <th>sibsp</th>
      <th>parch</th>
      <th>ticket</th>
      <th>fare</th>
      <th>cabin</th>
      <th>embarked</th>
      <th>boat</th>
      <th>body</th>
      <th>home.dest</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>1</td>
      <td>Allen, Miss. Elisabeth Walton</td>
      <td>female</td>
      <td>29</td>
      <td>0</td>
      <td>0</td>
      <td>24160</td>
      <td>211.3375</td>
      <td>B5</td>
      <td>S</td>
      <td>2</td>
      <td>?</td>
      <td>St Louis, MO</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>1</td>
      <td>Allison, Master. Hudson Trevor</td>
      <td>male</td>
      <td>0.9167</td>
      <td>1</td>
      <td>2</td>
      <td>113781</td>
      <td>151.55</td>
      <td>C22 C26</td>
      <td>S</td>
      <td>11</td>
      <td>?</td>
      <td>Montreal, PQ / Chesterville, ON</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1</td>
      <td>0</td>
      <td>Allison, Miss. Helen Loraine</td>
      <td>female</td>
      <td>2</td>
      <td>1</td>
      <td>2</td>
      <td>113781</td>
      <td>151.55</td>
      <td>C22 C26</td>
      <td>S</td>
      <td>?</td>
      <td>?</td>
      <td>Montreal, PQ / Chesterville, ON</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1</td>
      <td>0</td>
      <td>Allison, Mr. Hudson Joshua Creighton</td>
      <td>male</td>
      <td>30</td>
      <td>1</td>
      <td>2</td>
      <td>113781</td>
      <td>151.55</td>
      <td>C22 C26</td>
      <td>S</td>
      <td>?</td>
      <td>135</td>
      <td>Montreal, PQ / Chesterville, ON</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1</td>
      <td>0</td>
      <td>Allison, Mrs. Hudson J C (Bessie Waldo Daniels)</td>
      <td>female</td>
      <td>25</td>
      <td>1</td>
      <td>2</td>
      <td>113781</td>
      <td>151.55</td>
      <td>C22 C26</td>
      <td>S</td>
      <td>?</td>
      <td>?</td>
      <td>Montreal, PQ / Chesterville, ON</td>
    </tr>
  </tbody>
</table>
</div>



## read_csv with non-comma separators
The `netflix_titles.csv` file is actually pipe (`|`) separated.  We can tell `read_csv` to expect this using the `sep="|"` option. 

Additionally, the netflix dataset includes an index column as the very first column.  We can let `read_csv` know using `index_col=0`


```python
netflix = pd.read_csv("data/netflix_titles.csv", sep="|", index_col=0)
```


```python
netflix.info()
```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 8807 entries, 0 to 8806
    Data columns (total 12 columns):
     #   Column        Non-Null Count  Dtype 
    ---  ------        --------------  ----- 
     0   show_id       8807 non-null   object
     1   type          8807 non-null   object
     2   title         8807 non-null   object
     3   director      6173 non-null   object
     4   cast          7982 non-null   object
     5   country       7976 non-null   object
     6   date_added    8797 non-null   object
     7   release_year  8807 non-null   int64 
     8   rating        8803 non-null   object
     9   duration      8804 non-null   object
     10  listed_in     8807 non-null   object
     11  description   8807 non-null   object
    dtypes: int64(1), object(11)
    memory usage: 894.5+ KB
    


```python
netflix.head()
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
      <th>show_id</th>
      <th>type</th>
      <th>title</th>
      <th>director</th>
      <th>cast</th>
      <th>country</th>
      <th>date_added</th>
      <th>release_year</th>
      <th>rating</th>
      <th>duration</th>
      <th>listed_in</th>
      <th>description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>s1</td>
      <td>Movie</td>
      <td>Dick Johnson Is Dead</td>
      <td>Kirsten Johnson</td>
      <td>NaN</td>
      <td>United States</td>
      <td>September 25, 2021</td>
      <td>2020</td>
      <td>PG-13</td>
      <td>90 min</td>
      <td>Documentaries</td>
      <td>As her father nears the end of his life, filmm...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>s2</td>
      <td>TV Show</td>
      <td>Blood &amp; Water</td>
      <td>NaN</td>
      <td>Ama Qamata, Khosi Ngema, Gail Mabalane, Thaban...</td>
      <td>South Africa</td>
      <td>September 24, 2021</td>
      <td>2021</td>
      <td>TV-MA</td>
      <td>2 Seasons</td>
      <td>International TV Shows, TV Dramas, TV Mysteries</td>
      <td>After crossing paths at a party, a Cape Town t...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>s3</td>
      <td>TV Show</td>
      <td>Ganglands</td>
      <td>Julien Leclercq</td>
      <td>Sami Bouajila, Tracy Gotoas, Samuel Jouy, Nabi...</td>
      <td>NaN</td>
      <td>September 24, 2021</td>
      <td>2021</td>
      <td>TV-MA</td>
      <td>1 Season</td>
      <td>Crime TV Shows, International TV Shows, TV Act...</td>
      <td>To protect his family from a powerful drug lor...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>s4</td>
      <td>TV Show</td>
      <td>Jailbirds New Orleans</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>September 24, 2021</td>
      <td>2021</td>
      <td>TV-MA</td>
      <td>1 Season</td>
      <td>Docuseries, Reality TV</td>
      <td>Feuds, flirtations and toilet talk go down amo...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>s5</td>
      <td>TV Show</td>
      <td>Kota Factory</td>
      <td>NaN</td>
      <td>Mayur More, Jitendra Kumar, Ranjan Raj, Alam K...</td>
      <td>India</td>
      <td>September 24, 2021</td>
      <td>2021</td>
      <td>TV-MA</td>
      <td>2 Seasons</td>
      <td>International TV Shows, Romantic TV Shows, TV ...</td>
      <td>In a city of coaching centers known to train I...</td>
    </tr>
  </tbody>
</table>
</div>



## Proving Column Names

We can provide a list of custom column names to `read_csv` using the `names` parameter.  Additionally, we need to specify `header=0` to tell `read_csv` that the file still contains the original headers on the first line and that it should ignore them!


```python
names = ['sumlev', 'region', 'division', 'state', 'name', 'census2010pop', 'estimatesbase2010', 'popestimate2010', 'popestimate2011', 'popestimate2012', 'popestimate2013', 'popestimate2014', 'popestimate2015', 'popestimate2016', 'popestimate2017', 'popestimate2018', 'popestimate2019', 'popestimate042020', 'popestimate2020']
state_pops = pd.read_csv("data/nst-est2020.csv", names=names, header=0)
state_pops
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
      <th>sumlev</th>
      <th>region</th>
      <th>division</th>
      <th>state</th>
      <th>name</th>
      <th>census2010pop</th>
      <th>estimatesbase2010</th>
      <th>popestimate2010</th>
      <th>popestimate2011</th>
      <th>popestimate2012</th>
      <th>popestimate2013</th>
      <th>popestimate2014</th>
      <th>popestimate2015</th>
      <th>popestimate2016</th>
      <th>popestimate2017</th>
      <th>popestimate2018</th>
      <th>popestimate2019</th>
      <th>popestimate042020</th>
      <th>popestimate2020</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>10</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>United States</td>
      <td>308745538</td>
      <td>308758105</td>
      <td>309327143</td>
      <td>311583481</td>
      <td>313877662</td>
      <td>316059947</td>
      <td>318386329</td>
      <td>320738994</td>
      <td>323071755</td>
      <td>325122128</td>
      <td>326838199</td>
      <td>328329953</td>
      <td>329398742</td>
      <td>329484123</td>
    </tr>
    <tr>
      <th>1</th>
      <td>20</td>
      <td>1</td>
      <td>0</td>
      <td>0</td>
      <td>Northeast Region</td>
      <td>55317240</td>
      <td>55318414</td>
      <td>55380764</td>
      <td>55608318</td>
      <td>55782661</td>
      <td>55912775</td>
      <td>56021339</td>
      <td>56052790</td>
      <td>56063777</td>
      <td>56083383</td>
      <td>56084543</td>
      <td>56002934</td>
      <td>55924275</td>
      <td>55849869</td>
    </tr>
    <tr>
      <th>2</th>
      <td>20</td>
      <td>2</td>
      <td>0</td>
      <td>0</td>
      <td>Midwest Region</td>
      <td>66927001</td>
      <td>66929737</td>
      <td>66975328</td>
      <td>67164092</td>
      <td>67348275</td>
      <td>67576524</td>
      <td>67765576</td>
      <td>67885682</td>
      <td>68018175</td>
      <td>68160342</td>
      <td>68263019</td>
      <td>68340091</td>
      <td>68357895</td>
      <td>68316744</td>
    </tr>
    <tr>
      <th>3</th>
      <td>20</td>
      <td>3</td>
      <td>0</td>
      <td>0</td>
      <td>South Region</td>
      <td>114555744</td>
      <td>114563042</td>
      <td>114869421</td>
      <td>116019483</td>
      <td>117264196</td>
      <td>118397213</td>
      <td>119666248</td>
      <td>121049223</td>
      <td>122419547</td>
      <td>123611036</td>
      <td>124649156</td>
      <td>125686544</td>
      <td>126494232</td>
      <td>126662754</td>
    </tr>
    <tr>
      <th>4</th>
      <td>20</td>
      <td>4</td>
      <td>0</td>
      <td>0</td>
      <td>West Region</td>
      <td>71945553</td>
      <td>71946912</td>
      <td>72101630</td>
      <td>72791588</td>
      <td>73482530</td>
      <td>74173435</td>
      <td>74933166</td>
      <td>75751299</td>
      <td>76570256</td>
      <td>77267367</td>
      <td>77841481</td>
      <td>78300384</td>
      <td>78622340</td>
      <td>78654756</td>
    </tr>
    <tr>
      <th>5</th>
      <td>40</td>
      <td>3</td>
      <td>6</td>
      <td>1</td>
      <td>Alabama</td>
      <td>4779736</td>
      <td>4780118</td>
      <td>4785514</td>
      <td>4799642</td>
      <td>4816632</td>
      <td>4831586</td>
      <td>4843737</td>
      <td>4854803</td>
      <td>4866824</td>
      <td>4877989</td>
      <td>4891628</td>
      <td>4907965</td>
      <td>4920706</td>
      <td>4921532</td>
    </tr>
    <tr>
      <th>6</th>
      <td>40</td>
      <td>4</td>
      <td>9</td>
      <td>2</td>
      <td>Alaska</td>
      <td>710231</td>
      <td>710246</td>
      <td>713982</td>
      <td>722349</td>
      <td>730810</td>
      <td>737626</td>
      <td>737075</td>
      <td>738430</td>
      <td>742575</td>
      <td>740983</td>
      <td>736624</td>
      <td>733603</td>
      <td>732074</td>
      <td>731158</td>
    </tr>
    <tr>
      <th>7</th>
      <td>40</td>
      <td>4</td>
      <td>8</td>
      <td>4</td>
      <td>Arizona</td>
      <td>6392017</td>
      <td>6392292</td>
      <td>6407342</td>
      <td>6473416</td>
      <td>6556344</td>
      <td>6634690</td>
      <td>6732873</td>
      <td>6832810</td>
      <td>6944767</td>
      <td>7048088</td>
      <td>7164228</td>
      <td>7291843</td>
      <td>7393900</td>
      <td>7421401</td>
    </tr>
    <tr>
      <th>8</th>
      <td>40</td>
      <td>3</td>
      <td>7</td>
      <td>5</td>
      <td>Arkansas</td>
      <td>2915918</td>
      <td>2916029</td>
      <td>2921998</td>
      <td>2941038</td>
      <td>2952876</td>
      <td>2960459</td>
      <td>2968759</td>
      <td>2979732</td>
      <td>2991815</td>
      <td>3003855</td>
      <td>3012161</td>
      <td>3020985</td>
      <td>3029672</td>
      <td>3030522</td>
    </tr>
    <tr>
      <th>9</th>
      <td>40</td>
      <td>4</td>
      <td>9</td>
      <td>6</td>
      <td>California</td>
      <td>37253956</td>
      <td>37254522</td>
      <td>37319550</td>
      <td>37636311</td>
      <td>37944551</td>
      <td>38253768</td>
      <td>38586706</td>
      <td>38904296</td>
      <td>39149186</td>
      <td>39337785</td>
      <td>39437463</td>
      <td>39437610</td>
      <td>39418894</td>
      <td>39368078</td>
    </tr>
    <tr>
      <th>10</th>
      <td>40</td>
      <td>4</td>
      <td>8</td>
      <td>8</td>
      <td>Colorado</td>
      <td>5029196</td>
      <td>5029319</td>
      <td>5047539</td>
      <td>5121900</td>
      <td>5193660</td>
      <td>5270774</td>
      <td>5352637</td>
      <td>5454328</td>
      <td>5543844</td>
      <td>5617421</td>
      <td>5697155</td>
      <td>5758486</td>
      <td>5798266</td>
      <td>5807719</td>
    </tr>
    <tr>
      <th>11</th>
      <td>40</td>
      <td>1</td>
      <td>1</td>
      <td>9</td>
      <td>Connecticut</td>
      <td>3574097</td>
      <td>3574151</td>
      <td>3579173</td>
      <td>3588632</td>
      <td>3595211</td>
      <td>3595792</td>
      <td>3595697</td>
      <td>3588561</td>
      <td>3579830</td>
      <td>3575324</td>
      <td>3574561</td>
      <td>3566022</td>
      <td>3561494</td>
      <td>3557006</td>
    </tr>
    <tr>
      <th>12</th>
      <td>40</td>
      <td>3</td>
      <td>5</td>
      <td>10</td>
      <td>Delaware</td>
      <td>897934</td>
      <td>897947</td>
      <td>899647</td>
      <td>907590</td>
      <td>915518</td>
      <td>924062</td>
      <td>933131</td>
      <td>942065</td>
      <td>949989</td>
      <td>957942</td>
      <td>966985</td>
      <td>976668</td>
      <td>984899</td>
      <td>986809</td>
    </tr>
    <tr>
      <th>13</th>
      <td>40</td>
      <td>3</td>
      <td>5</td>
      <td>11</td>
      <td>District of Columbia</td>
      <td>601723</td>
      <td>601767</td>
      <td>605282</td>
      <td>620290</td>
      <td>635737</td>
      <td>651559</td>
      <td>663603</td>
      <td>677014</td>
      <td>687576</td>
      <td>697079</td>
      <td>704147</td>
      <td>708253</td>
      <td>712185</td>
      <td>712816</td>
    </tr>
    <tr>
      <th>14</th>
      <td>40</td>
      <td>3</td>
      <td>5</td>
      <td>12</td>
      <td>Florida</td>
      <td>18801310</td>
      <td>18804589</td>
      <td>18846143</td>
      <td>19055607</td>
      <td>19302016</td>
      <td>19551678</td>
      <td>19853880</td>
      <td>20219111</td>
      <td>20627237</td>
      <td>20977089</td>
      <td>21254926</td>
      <td>21492056</td>
      <td>21688239</td>
      <td>21733312</td>
    </tr>
    <tr>
      <th>15</th>
      <td>40</td>
      <td>3</td>
      <td>5</td>
      <td>13</td>
      <td>Georgia</td>
      <td>9687653</td>
      <td>9688737</td>
      <td>9712209</td>
      <td>9803630</td>
      <td>9903580</td>
      <td>9975592</td>
      <td>10071204</td>
      <td>10183353</td>
      <td>10308442</td>
      <td>10417031</td>
      <td>10519389</td>
      <td>10628020</td>
      <td>10695662</td>
      <td>10710017</td>
    </tr>
    <tr>
      <th>16</th>
      <td>40</td>
      <td>4</td>
      <td>9</td>
      <td>15</td>
      <td>Hawaii</td>
      <td>1360301</td>
      <td>1360304</td>
      <td>1364004</td>
      <td>1379562</td>
      <td>1395199</td>
      <td>1408822</td>
      <td>1415335</td>
      <td>1422999</td>
      <td>1428885</td>
      <td>1425763</td>
      <td>1423102</td>
      <td>1415615</td>
      <td>1410587</td>
      <td>1407006</td>
    </tr>
    <tr>
      <th>17</th>
      <td>40</td>
      <td>4</td>
      <td>8</td>
      <td>16</td>
      <td>Idaho</td>
      <td>1567582</td>
      <td>1567658</td>
      <td>1570819</td>
      <td>1584272</td>
      <td>1595910</td>
      <td>1612053</td>
      <td>1632248</td>
      <td>1652495</td>
      <td>1684036</td>
      <td>1719745</td>
      <td>1752074</td>
      <td>1789060</td>
      <td>1818238</td>
      <td>1826913</td>
    </tr>
    <tr>
      <th>18</th>
      <td>40</td>
      <td>2</td>
      <td>3</td>
      <td>17</td>
      <td>Illinois</td>
      <td>12830632</td>
      <td>12831572</td>
      <td>12840545</td>
      <td>12867783</td>
      <td>12883029</td>
      <td>12895778</td>
      <td>12885092</td>
      <td>12859585</td>
      <td>12821709</td>
      <td>12779893</td>
      <td>12724685</td>
      <td>12667017</td>
      <td>12615162</td>
      <td>12587530</td>
    </tr>
    <tr>
      <th>19</th>
      <td>40</td>
      <td>2</td>
      <td>3</td>
      <td>18</td>
      <td>Indiana</td>
      <td>6483802</td>
      <td>6484050</td>
      <td>6490555</td>
      <td>6517250</td>
      <td>6538989</td>
      <td>6570575</td>
      <td>6596019</td>
      <td>6611442</td>
      <td>6637898</td>
      <td>6662068</td>
      <td>6698481</td>
      <td>6731010</td>
      <td>6752183</td>
      <td>6754953</td>
    </tr>
    <tr>
      <th>20</th>
      <td>40</td>
      <td>2</td>
      <td>4</td>
      <td>19</td>
      <td>Iowa</td>
      <td>3046355</td>
      <td>3046877</td>
      <td>3050819</td>
      <td>3066772</td>
      <td>3076844</td>
      <td>3093935</td>
      <td>3110643</td>
      <td>3122541</td>
      <td>3133210</td>
      <td>3143734</td>
      <td>3149900</td>
      <td>3159596</td>
      <td>3164115</td>
      <td>3163561</td>
    </tr>
    <tr>
      <th>21</th>
      <td>40</td>
      <td>2</td>
      <td>4</td>
      <td>20</td>
      <td>Kansas</td>
      <td>2853118</td>
      <td>2853120</td>
      <td>2858266</td>
      <td>2869677</td>
      <td>2886024</td>
      <td>2894306</td>
      <td>2901861</td>
      <td>2910717</td>
      <td>2912977</td>
      <td>2910892</td>
      <td>2912748</td>
      <td>2912635</td>
      <td>2915024</td>
      <td>2913805</td>
    </tr>
    <tr>
      <th>22</th>
      <td>40</td>
      <td>3</td>
      <td>6</td>
      <td>21</td>
      <td>Kentucky</td>
      <td>4339367</td>
      <td>4339330</td>
      <td>4348464</td>
      <td>4370817</td>
      <td>4387865</td>
      <td>4406906</td>
      <td>4416992</td>
      <td>4429126</td>
      <td>4440306</td>
      <td>4455590</td>
      <td>4464273</td>
      <td>4472345</td>
      <td>4477899</td>
      <td>4477251</td>
    </tr>
    <tr>
      <th>23</th>
      <td>40</td>
      <td>3</td>
      <td>7</td>
      <td>22</td>
      <td>Louisiana</td>
      <td>4533372</td>
      <td>4533500</td>
      <td>4544635</td>
      <td>4576244</td>
      <td>4602067</td>
      <td>4626040</td>
      <td>4645938</td>
      <td>4666998</td>
      <td>4681346</td>
      <td>4673673</td>
      <td>4664450</td>
      <td>4658285</td>
      <td>4650984</td>
      <td>4645318</td>
    </tr>
    <tr>
      <th>24</th>
      <td>40</td>
      <td>1</td>
      <td>1</td>
      <td>23</td>
      <td>Maine</td>
      <td>1328361</td>
      <td>1328354</td>
      <td>1327651</td>
      <td>1328473</td>
      <td>1328094</td>
      <td>1328543</td>
      <td>1331217</td>
      <td>1329098</td>
      <td>1332348</td>
      <td>1335743</td>
      <td>1340123</td>
      <td>1345770</td>
      <td>1349647</td>
      <td>1350141</td>
    </tr>
    <tr>
      <th>25</th>
      <td>40</td>
      <td>3</td>
      <td>5</td>
      <td>24</td>
      <td>Maryland</td>
      <td>5773552</td>
      <td>5773787</td>
      <td>5788784</td>
      <td>5840241</td>
      <td>5888375</td>
      <td>5925197</td>
      <td>5960064</td>
      <td>5988528</td>
      <td>6007014</td>
      <td>6028186</td>
      <td>6042153</td>
      <td>6054954</td>
      <td>6059529</td>
      <td>6055802</td>
    </tr>
    <tr>
      <th>26</th>
      <td>40</td>
      <td>1</td>
      <td>1</td>
      <td>25</td>
      <td>Massachusetts</td>
      <td>6547629</td>
      <td>6547788</td>
      <td>6566440</td>
      <td>6614218</td>
      <td>6664269</td>
      <td>6715158</td>
      <td>6764864</td>
      <td>6797484</td>
      <td>6827280</td>
      <td>6863560</td>
      <td>6885720</td>
      <td>6894883</td>
      <td>6898116</td>
      <td>6893574</td>
    </tr>
    <tr>
      <th>27</th>
      <td>40</td>
      <td>2</td>
      <td>3</td>
      <td>26</td>
      <td>Michigan</td>
      <td>9883640</td>
      <td>9884112</td>
      <td>9877597</td>
      <td>9883053</td>
      <td>9898289</td>
      <td>9914802</td>
      <td>9932033</td>
      <td>9934483</td>
      <td>9954117</td>
      <td>9976752</td>
      <td>9987286</td>
      <td>9984795</td>
      <td>9976330</td>
      <td>9966555</td>
    </tr>
    <tr>
      <th>28</th>
      <td>40</td>
      <td>2</td>
      <td>4</td>
      <td>27</td>
      <td>Minnesota</td>
      <td>5303925</td>
      <td>5303933</td>
      <td>5310934</td>
      <td>5346620</td>
      <td>5377500</td>
      <td>5414722</td>
      <td>5452665</td>
      <td>5484002</td>
      <td>5525360</td>
      <td>5569283</td>
      <td>5608762</td>
      <td>5640053</td>
      <td>5655855</td>
      <td>5657342</td>
    </tr>
    <tr>
      <th>29</th>
      <td>40</td>
      <td>3</td>
      <td>6</td>
      <td>28</td>
      <td>Mississippi</td>
      <td>2967297</td>
      <td>2968129</td>
      <td>2970615</td>
      <td>2979147</td>
      <td>2984599</td>
      <td>2989839</td>
      <td>2991892</td>
      <td>2990231</td>
      <td>2990595</td>
      <td>2990674</td>
      <td>2982879</td>
      <td>2978227</td>
      <td>2971253</td>
      <td>2966786</td>
    </tr>
    <tr>
      <th>30</th>
      <td>40</td>
      <td>2</td>
      <td>4</td>
      <td>29</td>
      <td>Missouri</td>
      <td>5988927</td>
      <td>5988941</td>
      <td>5996089</td>
      <td>6011182</td>
      <td>6026027</td>
      <td>6042989</td>
      <td>6059130</td>
      <td>6075411</td>
      <td>6091384</td>
      <td>6111382</td>
      <td>6125986</td>
      <td>6140475</td>
      <td>6151737</td>
      <td>6151548</td>
    </tr>
    <tr>
      <th>31</th>
      <td>40</td>
      <td>4</td>
      <td>8</td>
      <td>30</td>
      <td>Montana</td>
      <td>989415</td>
      <td>989400</td>
      <td>990730</td>
      <td>997518</td>
      <td>1004168</td>
      <td>1014158</td>
      <td>1022657</td>
      <td>1031495</td>
      <td>1042137</td>
      <td>1053862</td>
      <td>1061818</td>
      <td>1070123</td>
      <td>1078405</td>
      <td>1080577</td>
    </tr>
    <tr>
      <th>32</th>
      <td>40</td>
      <td>2</td>
      <td>4</td>
      <td>31</td>
      <td>Nebraska</td>
      <td>1826341</td>
      <td>1826311</td>
      <td>1829591</td>
      <td>1840914</td>
      <td>1853691</td>
      <td>1865813</td>
      <td>1879955</td>
      <td>1892059</td>
      <td>1906483</td>
      <td>1916998</td>
      <td>1925512</td>
      <td>1932571</td>
      <td>1937258</td>
      <td>1937552</td>
    </tr>
    <tr>
      <th>33</th>
      <td>40</td>
      <td>4</td>
      <td>8</td>
      <td>32</td>
      <td>Nevada</td>
      <td>2700551</td>
      <td>2700683</td>
      <td>2702483</td>
      <td>2713114</td>
      <td>2744670</td>
      <td>2776956</td>
      <td>2818935</td>
      <td>2868531</td>
      <td>2919555</td>
      <td>2972097</td>
      <td>3030725</td>
      <td>3090771</td>
      <td>3128500</td>
      <td>3138259</td>
    </tr>
    <tr>
      <th>34</th>
      <td>40</td>
      <td>1</td>
      <td>1</td>
      <td>33</td>
      <td>New Hampshire</td>
      <td>1316470</td>
      <td>1316457</td>
      <td>1316807</td>
      <td>1320444</td>
      <td>1324677</td>
      <td>1327272</td>
      <td>1334257</td>
      <td>1337480</td>
      <td>1343694</td>
      <td>1350395</td>
      <td>1355064</td>
      <td>1360783</td>
      <td>1365533</td>
      <td>1366275</td>
    </tr>
    <tr>
      <th>35</th>
      <td>40</td>
      <td>1</td>
      <td>2</td>
      <td>34</td>
      <td>New Jersey</td>
      <td>8791894</td>
      <td>8791959</td>
      <td>8799451</td>
      <td>8828552</td>
      <td>8845671</td>
      <td>8857821</td>
      <td>8867277</td>
      <td>8870312</td>
      <td>8873584</td>
      <td>8888147</td>
      <td>8891730</td>
      <td>8891258</td>
      <td>8890883</td>
      <td>8882371</td>
    </tr>
    <tr>
      <th>36</th>
      <td>40</td>
      <td>4</td>
      <td>8</td>
      <td>35</td>
      <td>New Mexico</td>
      <td>2059179</td>
      <td>2059199</td>
      <td>2064614</td>
      <td>2080707</td>
      <td>2087715</td>
      <td>2092833</td>
      <td>2090236</td>
      <td>2090071</td>
      <td>2092555</td>
      <td>2092844</td>
      <td>2093754</td>
      <td>2099634</td>
      <td>2106117</td>
      <td>2106319</td>
    </tr>
    <tr>
      <th>37</th>
      <td>40</td>
      <td>1</td>
      <td>2</td>
      <td>36</td>
      <td>New York</td>
      <td>19378102</td>
      <td>19378117</td>
      <td>19399956</td>
      <td>19499921</td>
      <td>19574362</td>
      <td>19626488</td>
      <td>19653431</td>
      <td>19657321</td>
      <td>19636391</td>
      <td>19593849</td>
      <td>19544098</td>
      <td>19463131</td>
      <td>19382373</td>
      <td>19336776</td>
    </tr>
    <tr>
      <th>38</th>
      <td>40</td>
      <td>3</td>
      <td>5</td>
      <td>37</td>
      <td>North Carolina</td>
      <td>9535483</td>
      <td>9535762</td>
      <td>9574586</td>
      <td>9658913</td>
      <td>9751810</td>
      <td>9846717</td>
      <td>9937295</td>
      <td>10037218</td>
      <td>10161802</td>
      <td>10275758</td>
      <td>10391358</td>
      <td>10501384</td>
      <td>10581885</td>
      <td>10600823</td>
    </tr>
    <tr>
      <th>39</th>
      <td>40</td>
      <td>2</td>
      <td>4</td>
      <td>38</td>
      <td>North Dakota</td>
      <td>672591</td>
      <td>672575</td>
      <td>674752</td>
      <td>685526</td>
      <td>702227</td>
      <td>723149</td>
      <td>738736</td>
      <td>755537</td>
      <td>756114</td>
      <td>756755</td>
      <td>760062</td>
      <td>763724</td>
      <td>765224</td>
      <td>765309</td>
    </tr>
    <tr>
      <th>40</th>
      <td>40</td>
      <td>2</td>
      <td>3</td>
      <td>39</td>
      <td>Ohio</td>
      <td>11536504</td>
      <td>11536763</td>
      <td>11539449</td>
      <td>11545735</td>
      <td>11550971</td>
      <td>11579692</td>
      <td>11606573</td>
      <td>11622315</td>
      <td>11640060</td>
      <td>11665706</td>
      <td>11680892</td>
      <td>11696507</td>
      <td>11699855</td>
      <td>11693217</td>
    </tr>
    <tr>
      <th>41</th>
      <td>40</td>
      <td>3</td>
      <td>7</td>
      <td>40</td>
      <td>Oklahoma</td>
      <td>3751351</td>
      <td>3751582</td>
      <td>3760014</td>
      <td>3788824</td>
      <td>3819320</td>
      <td>3853891</td>
      <td>3879187</td>
      <td>3910518</td>
      <td>3928143</td>
      <td>3933602</td>
      <td>3943488</td>
      <td>3960676</td>
      <td>3977682</td>
      <td>3980783</td>
    </tr>
    <tr>
      <th>42</th>
      <td>40</td>
      <td>4</td>
      <td>9</td>
      <td>41</td>
      <td>Oregon</td>
      <td>3831074</td>
      <td>3831083</td>
      <td>3837614</td>
      <td>3872672</td>
      <td>3900102</td>
      <td>3924110</td>
      <td>3965447</td>
      <td>4018542</td>
      <td>4093271</td>
      <td>4147294</td>
      <td>4183538</td>
      <td>4216116</td>
      <td>4237408</td>
      <td>4241507</td>
    </tr>
    <tr>
      <th>43</th>
      <td>40</td>
      <td>1</td>
      <td>2</td>
      <td>42</td>
      <td>Pennsylvania</td>
      <td>12702379</td>
      <td>12702891</td>
      <td>12711406</td>
      <td>12747052</td>
      <td>12769123</td>
      <td>12779538</td>
      <td>12792392</td>
      <td>12789838</td>
      <td>12788468</td>
      <td>12794679</td>
      <td>12809107</td>
      <td>12798883</td>
      <td>12794404</td>
      <td>12783254</td>
    </tr>
    <tr>
      <th>44</th>
      <td>40</td>
      <td>1</td>
      <td>1</td>
      <td>44</td>
      <td>Rhode Island</td>
      <td>1052567</td>
      <td>1052970</td>
      <td>1053994</td>
      <td>1053829</td>
      <td>1054893</td>
      <td>1055560</td>
      <td>1056511</td>
      <td>1056886</td>
      <td>1057816</td>
      <td>1056554</td>
      <td>1059338</td>
      <td>1058158</td>
      <td>1058004</td>
      <td>1057125</td>
    </tr>
    <tr>
      <th>45</th>
      <td>40</td>
      <td>3</td>
      <td>5</td>
      <td>45</td>
      <td>South Carolina</td>
      <td>4625364</td>
      <td>4625358</td>
      <td>4635846</td>
      <td>4672655</td>
      <td>4719027</td>
      <td>4766469</td>
      <td>4826858</td>
      <td>4896006</td>
      <td>4963031</td>
      <td>5027102</td>
      <td>5091702</td>
      <td>5157702</td>
      <td>5205864</td>
      <td>5218040</td>
    </tr>
    <tr>
      <th>46</th>
      <td>40</td>
      <td>2</td>
      <td>4</td>
      <td>46</td>
      <td>South Dakota</td>
      <td>814180</td>
      <td>814198</td>
      <td>816193</td>
      <td>823740</td>
      <td>833859</td>
      <td>842751</td>
      <td>849670</td>
      <td>854663</td>
      <td>863693</td>
      <td>873732</td>
      <td>879386</td>
      <td>887127</td>
      <td>891688</td>
      <td>892717</td>
    </tr>
    <tr>
      <th>47</th>
      <td>40</td>
      <td>3</td>
      <td>6</td>
      <td>47</td>
      <td>Tennessee</td>
      <td>6346105</td>
      <td>6346281</td>
      <td>6355518</td>
      <td>6400298</td>
      <td>6455752</td>
      <td>6496943</td>
      <td>6544617</td>
      <td>6595354</td>
      <td>6651277</td>
      <td>6714748</td>
      <td>6778180</td>
      <td>6830325</td>
      <td>6875939</td>
      <td>6886834</td>
    </tr>
    <tr>
      <th>48</th>
      <td>40</td>
      <td>3</td>
      <td>7</td>
      <td>48</td>
      <td>Texas</td>
      <td>25145561</td>
      <td>25146072</td>
      <td>25241897</td>
      <td>25645504</td>
      <td>26084120</td>
      <td>26479646</td>
      <td>26963092</td>
      <td>27468531</td>
      <td>27914064</td>
      <td>28291024</td>
      <td>28624564</td>
      <td>28986794</td>
      <td>29286467</td>
      <td>29360759</td>
    </tr>
    <tr>
      <th>49</th>
      <td>40</td>
      <td>4</td>
      <td>8</td>
      <td>49</td>
      <td>Utah</td>
      <td>2763885</td>
      <td>2763891</td>
      <td>2775413</td>
      <td>2814797</td>
      <td>2854146</td>
      <td>2898773</td>
      <td>2938327</td>
      <td>2983626</td>
      <td>3044241</td>
      <td>3103540</td>
      <td>3155153</td>
      <td>3203383</td>
      <td>3239542</td>
      <td>3249879</td>
    </tr>
    <tr>
      <th>50</th>
      <td>40</td>
      <td>1</td>
      <td>1</td>
      <td>50</td>
      <td>Vermont</td>
      <td>625741</td>
      <td>625727</td>
      <td>625886</td>
      <td>627197</td>
      <td>626361</td>
      <td>626603</td>
      <td>625693</td>
      <td>625810</td>
      <td>624366</td>
      <td>625132</td>
      <td>624802</td>
      <td>624046</td>
      <td>623821</td>
      <td>623347</td>
    </tr>
    <tr>
      <th>51</th>
      <td>40</td>
      <td>3</td>
      <td>5</td>
      <td>51</td>
      <td>Virginia</td>
      <td>8001024</td>
      <td>8001046</td>
      <td>8024004</td>
      <td>8102437</td>
      <td>8187456</td>
      <td>8255861</td>
      <td>8315430</td>
      <td>8367303</td>
      <td>8417651</td>
      <td>8471011</td>
      <td>8510920</td>
      <td>8556642</td>
      <td>8587217</td>
      <td>8590563</td>
    </tr>
    <tr>
      <th>52</th>
      <td>40</td>
      <td>4</td>
      <td>9</td>
      <td>53</td>
      <td>Washington</td>
      <td>6724540</td>
      <td>6724540</td>
      <td>6743009</td>
      <td>6827479</td>
      <td>6898599</td>
      <td>6966252</td>
      <td>7057531</td>
      <td>7167287</td>
      <td>7299961</td>
      <td>7427951</td>
      <td>7526793</td>
      <td>7614024</td>
      <td>7678379</td>
      <td>7693612</td>
    </tr>
    <tr>
      <th>53</th>
      <td>40</td>
      <td>3</td>
      <td>5</td>
      <td>54</td>
      <td>West Virginia</td>
      <td>1852994</td>
      <td>1853008</td>
      <td>1854265</td>
      <td>1856606</td>
      <td>1857446</td>
      <td>1854768</td>
      <td>1850569</td>
      <td>1843332</td>
      <td>1832435</td>
      <td>1818683</td>
      <td>1805953</td>
      <td>1795263</td>
      <td>1788150</td>
      <td>1784787</td>
    </tr>
    <tr>
      <th>54</th>
      <td>40</td>
      <td>2</td>
      <td>3</td>
      <td>55</td>
      <td>Wisconsin</td>
      <td>5686986</td>
      <td>5687285</td>
      <td>5690538</td>
      <td>5705840</td>
      <td>5720825</td>
      <td>5738012</td>
      <td>5753199</td>
      <td>5762927</td>
      <td>5775170</td>
      <td>5793147</td>
      <td>5809319</td>
      <td>5824581</td>
      <td>5833464</td>
      <td>5832655</td>
    </tr>
    <tr>
      <th>55</th>
      <td>40</td>
      <td>4</td>
      <td>8</td>
      <td>56</td>
      <td>Wyoming</td>
      <td>563626</td>
      <td>563775</td>
      <td>564531</td>
      <td>567491</td>
      <td>576656</td>
      <td>582620</td>
      <td>583159</td>
      <td>586389</td>
      <td>585243</td>
      <td>579994</td>
      <td>579054</td>
      <td>580116</td>
      <td>582030</td>
      <td>582328</td>
    </tr>
    <tr>
      <th>56</th>
      <td>40</td>
      <td>X</td>
      <td>X</td>
      <td>72</td>
      <td>Puerto Rico</td>
      <td>3725789</td>
      <td>3726157</td>
      <td>3721525</td>
      <td>3678732</td>
      <td>3634488</td>
      <td>3593077</td>
      <td>3534874</td>
      <td>3473232</td>
      <td>3406672</td>
      <td>3325284</td>
      <td>3193344</td>
      <td>3193553</td>
      <td>3167851</td>
      <td>3159343</td>
    </tr>
  </tbody>
</table>
</div>


