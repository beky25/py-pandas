

```python
import pandas as pd
import json
import os
```


```python
panjson=os.path.join('purchase_data.json')
```


```python
#Read json data into a variable with open(panjson) as json_d:
with open(panjson) as json_d:
    heroes = pd.read_json(json_d)
heroes
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
      <th>Age</th>
      <th>Gender</th>
      <th>Item ID</th>
      <th>Item Name</th>
      <th>Price</th>
      <th>SN</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>38</td>
      <td>Male</td>
      <td>165</td>
      <td>Bone Crushing Silver Skewer</td>
      <td>3.37</td>
      <td>Aelalis34</td>
    </tr>
    <tr>
      <th>1</th>
      <td>21</td>
      <td>Male</td>
      <td>119</td>
      <td>Stormbringer, Dark Blade of Ending Misery</td>
      <td>2.32</td>
      <td>Eolo46</td>
    </tr>
    <tr>
      <th>2</th>
      <td>34</td>
      <td>Male</td>
      <td>174</td>
      <td>Primitive Blade</td>
      <td>2.46</td>
      <td>Assastnya25</td>
    </tr>
    <tr>
      <th>3</th>
      <td>21</td>
      <td>Male</td>
      <td>92</td>
      <td>Final Critic</td>
      <td>1.36</td>
      <td>Pheusrical25</td>
    </tr>
    <tr>
      <th>4</th>
      <td>23</td>
      <td>Male</td>
      <td>63</td>
      <td>Stormfury Mace</td>
      <td>1.27</td>
      <td>Aela59</td>
    </tr>
    <tr>
      <th>5</th>
      <td>20</td>
      <td>Male</td>
      <td>10</td>
      <td>Sleepwalker</td>
      <td>1.73</td>
      <td>Tanimnya91</td>
    </tr>
    <tr>
      <th>6</th>
      <td>20</td>
      <td>Male</td>
      <td>153</td>
      <td>Mercenary Sabre</td>
      <td>4.57</td>
      <td>Undjaskla97</td>
    </tr>
    <tr>
      <th>7</th>
      <td>29</td>
      <td>Female</td>
      <td>169</td>
      <td>Interrogator, Blood Blade of the Queen</td>
      <td>3.32</td>
      <td>Iathenudil29</td>
    </tr>
    <tr>
      <th>8</th>
      <td>25</td>
      <td>Male</td>
      <td>118</td>
      <td>Ghost Reaver, Longsword of Magic</td>
      <td>2.77</td>
      <td>Sondenasta63</td>
    </tr>
    <tr>
      <th>9</th>
      <td>31</td>
      <td>Male</td>
      <td>99</td>
      <td>Expiration, Warscythe Of Lost Worlds</td>
      <td>4.53</td>
      <td>Hilaerin92</td>
    </tr>
    <tr>
      <th>10</th>
      <td>24</td>
      <td>Male</td>
      <td>57</td>
      <td>Despair, Favor of Due Diligence</td>
      <td>3.81</td>
      <td>Chamosia29</td>
    </tr>
    <tr>
      <th>11</th>
      <td>20</td>
      <td>Male</td>
      <td>47</td>
      <td>Alpha, Reach of Ending Hope</td>
      <td>1.55</td>
      <td>Sally64</td>
    </tr>
    <tr>
      <th>12</th>
      <td>30</td>
      <td>Male</td>
      <td>81</td>
      <td>Dreamkiss</td>
      <td>4.06</td>
      <td>Iskossa88</td>
    </tr>
    <tr>
      <th>13</th>
      <td>23</td>
      <td>Male</td>
      <td>77</td>
      <td>Piety, Guardian of Riddles</td>
      <td>3.68</td>
      <td>Seorithstilis90</td>
    </tr>
    <tr>
      <th>14</th>
      <td>40</td>
      <td>Male</td>
      <td>44</td>
      <td>Bonecarvin Battle Axe</td>
      <td>2.46</td>
      <td>Sundast29</td>
    </tr>
    <tr>
      <th>15</th>
      <td>21</td>
      <td>Male</td>
      <td>96</td>
      <td>Blood-Forged Skeletal Spine</td>
      <td>4.77</td>
      <td>Haellysu29</td>
    </tr>
    <tr>
      <th>16</th>
      <td>22</td>
      <td>Female</td>
      <td>123</td>
      <td>Twilight's Carver</td>
      <td>1.14</td>
      <td>Sundista85</td>
    </tr>
    <tr>
      <th>17</th>
      <td>22</td>
      <td>Female</td>
      <td>59</td>
      <td>Lightning, Etcher of the King</td>
      <td>1.65</td>
      <td>Aenarap34</td>
    </tr>
    <tr>
      <th>18</th>
      <td>28</td>
      <td>Male</td>
      <td>91</td>
      <td>Celeste</td>
      <td>3.71</td>
      <td>Iskista88</td>
    </tr>
    <tr>
      <th>19</th>
      <td>31</td>
      <td>Male</td>
      <td>177</td>
      <td>Winterthorn, Defender of Shifting Worlds</td>
      <td>4.89</td>
      <td>Assossa43</td>
    </tr>
    <tr>
      <th>20</th>
      <td>24</td>
      <td>Male</td>
      <td>78</td>
      <td>Glimmer, Ender of the Moon</td>
      <td>2.33</td>
      <td>Irith83</td>
    </tr>
    <tr>
      <th>21</th>
      <td>15</td>
      <td>Male</td>
      <td>3</td>
      <td>Phantomlight</td>
      <td>1.79</td>
      <td>Iaralrgue74</td>
    </tr>
    <tr>
      <th>22</th>
      <td>11</td>
      <td>Female</td>
      <td>11</td>
      <td>Brimstone</td>
      <td>2.52</td>
      <td>Deural48</td>
    </tr>
    <tr>
      <th>23</th>
      <td>19</td>
      <td>Male</td>
      <td>183</td>
      <td>Dragon's Greatsword</td>
      <td>2.36</td>
      <td>Chanosia65</td>
    </tr>
    <tr>
      <th>24</th>
      <td>11</td>
      <td>Male</td>
      <td>65</td>
      <td>Conqueror Adamantite Mace</td>
      <td>1.96</td>
      <td>Qarwen67</td>
    </tr>
    <tr>
      <th>25</th>
      <td>21</td>
      <td>Male</td>
      <td>63</td>
      <td>Stormfury Mace</td>
      <td>1.27</td>
      <td>Idai61</td>
    </tr>
    <tr>
      <th>26</th>
      <td>29</td>
      <td>Male</td>
      <td>132</td>
      <td>Persuasion</td>
      <td>3.90</td>
      <td>Aerithllora36</td>
    </tr>
    <tr>
      <th>27</th>
      <td>34</td>
      <td>Male</td>
      <td>106</td>
      <td>Crying Steel Sickle</td>
      <td>2.29</td>
      <td>Assastnya25</td>
    </tr>
    <tr>
      <th>28</th>
      <td>15</td>
      <td>Male</td>
      <td>49</td>
      <td>The Oculus, Token of Lost Worlds</td>
      <td>4.23</td>
      <td>Ilariarin45</td>
    </tr>
    <tr>
      <th>29</th>
      <td>16</td>
      <td>Female</td>
      <td>45</td>
      <td>Glinting Glass Edge</td>
      <td>2.46</td>
      <td>Phaedai25</td>
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
      <th>750</th>
      <td>23</td>
      <td>Male</td>
      <td>86</td>
      <td>Stormfury Lantern</td>
      <td>1.28</td>
      <td>Eollym91</td>
    </tr>
    <tr>
      <th>751</th>
      <td>26</td>
      <td>Female</td>
      <td>179</td>
      <td>Wolf, Promise of the Moonwalker</td>
      <td>1.88</td>
      <td>Lisjasksda68</td>
    </tr>
    <tr>
      <th>752</th>
      <td>15</td>
      <td>Female</td>
      <td>116</td>
      <td>Renewed Skeletal Katana</td>
      <td>2.37</td>
      <td>Yalostiphos68</td>
    </tr>
    <tr>
      <th>753</th>
      <td>20</td>
      <td>Male</td>
      <td>4</td>
      <td>Bloodlord's Fetish</td>
      <td>2.28</td>
      <td>Thryallym62</td>
    </tr>
    <tr>
      <th>754</th>
      <td>31</td>
      <td>Male</td>
      <td>104</td>
      <td>Gladiator's Glaive</td>
      <td>1.36</td>
      <td>Sondastan54</td>
    </tr>
    <tr>
      <th>755</th>
      <td>22</td>
      <td>Female</td>
      <td>179</td>
      <td>Wolf, Promise of the Moonwalker</td>
      <td>1.88</td>
      <td>Ailaesuir66</td>
    </tr>
    <tr>
      <th>756</th>
      <td>22</td>
      <td>Male</td>
      <td>6</td>
      <td>Rusty Skull</td>
      <td>1.20</td>
      <td>Siasri67</td>
    </tr>
    <tr>
      <th>757</th>
      <td>35</td>
      <td>Male</td>
      <td>11</td>
      <td>Brimstone</td>
      <td>2.52</td>
      <td>Seosri62</td>
    </tr>
    <tr>
      <th>758</th>
      <td>20</td>
      <td>Male</td>
      <td>122</td>
      <td>Unending Tyranny</td>
      <td>1.21</td>
      <td>Ryastycal90</td>
    </tr>
    <tr>
      <th>759</th>
      <td>19</td>
      <td>Male</td>
      <td>87</td>
      <td>Deluge, Edge of the West</td>
      <td>2.20</td>
      <td>Chanirrasta87</td>
    </tr>
    <tr>
      <th>760</th>
      <td>29</td>
      <td>Male</td>
      <td>81</td>
      <td>Dreamkiss</td>
      <td>4.06</td>
      <td>Aerithllora36</td>
    </tr>
    <tr>
      <th>761</th>
      <td>28</td>
      <td>Male</td>
      <td>175</td>
      <td>Woeful Adamantite Claymore</td>
      <td>1.24</td>
      <td>Raeduerin33</td>
    </tr>
    <tr>
      <th>762</th>
      <td>36</td>
      <td>Male</td>
      <td>52</td>
      <td>Hatred</td>
      <td>4.39</td>
      <td>Lisosiast26</td>
    </tr>
    <tr>
      <th>763</th>
      <td>27</td>
      <td>Other / Non-Disclosed</td>
      <td>48</td>
      <td>Rage, Legacy of the Lone Victor</td>
      <td>4.32</td>
      <td>Eurisuru25</td>
    </tr>
    <tr>
      <th>764</th>
      <td>25</td>
      <td>Male</td>
      <td>70</td>
      <td>Hope's End</td>
      <td>3.89</td>
      <td>Assassasda84</td>
    </tr>
    <tr>
      <th>765</th>
      <td>15</td>
      <td>Male</td>
      <td>13</td>
      <td>Serenity</td>
      <td>1.49</td>
      <td>Aerithnucal56</td>
    </tr>
    <tr>
      <th>766</th>
      <td>22</td>
      <td>Female</td>
      <td>84</td>
      <td>Arcane Gem</td>
      <td>2.23</td>
      <td>Nitherian58</td>
    </tr>
    <tr>
      <th>767</th>
      <td>20</td>
      <td>Male</td>
      <td>122</td>
      <td>Unending Tyranny</td>
      <td>1.21</td>
      <td>Hailaphos89</td>
    </tr>
    <tr>
      <th>768</th>
      <td>21</td>
      <td>Male</td>
      <td>158</td>
      <td>Darkheart, Butcher of the Champion</td>
      <td>3.56</td>
      <td>Chamucosda93</td>
    </tr>
    <tr>
      <th>769</th>
      <td>24</td>
      <td>Male</td>
      <td>73</td>
      <td>Ritual Mace</td>
      <td>3.74</td>
      <td>Frichilsasya78</td>
    </tr>
    <tr>
      <th>770</th>
      <td>22</td>
      <td>Male</td>
      <td>141</td>
      <td>Persuasion</td>
      <td>3.27</td>
      <td>Aenasu69</td>
    </tr>
    <tr>
      <th>771</th>
      <td>24</td>
      <td>Male</td>
      <td>25</td>
      <td>Hero Cane</td>
      <td>1.03</td>
      <td>Lassista97</td>
    </tr>
    <tr>
      <th>772</th>
      <td>15</td>
      <td>Male</td>
      <td>31</td>
      <td>Trickster</td>
      <td>2.07</td>
      <td>Sidap51</td>
    </tr>
    <tr>
      <th>773</th>
      <td>21</td>
      <td>Male</td>
      <td>44</td>
      <td>Bonecarvin Battle Axe</td>
      <td>2.46</td>
      <td>Chamadarsda63</td>
    </tr>
    <tr>
      <th>774</th>
      <td>24</td>
      <td>Male</td>
      <td>123</td>
      <td>Twilight's Carver</td>
      <td>1.14</td>
      <td>Lassassast73</td>
    </tr>
    <tr>
      <th>775</th>
      <td>22</td>
      <td>Male</td>
      <td>98</td>
      <td>Deadline, Voice Of Subtlety</td>
      <td>3.62</td>
      <td>Eural50</td>
    </tr>
    <tr>
      <th>776</th>
      <td>14</td>
      <td>Male</td>
      <td>104</td>
      <td>Gladiator's Glaive</td>
      <td>1.36</td>
      <td>Lirtossa78</td>
    </tr>
    <tr>
      <th>777</th>
      <td>20</td>
      <td>Male</td>
      <td>117</td>
      <td>Heartstriker, Legacy of the Light</td>
      <td>4.15</td>
      <td>Tillyrin30</td>
    </tr>
    <tr>
      <th>778</th>
      <td>20</td>
      <td>Male</td>
      <td>75</td>
      <td>Brutality Ivory Warmace</td>
      <td>1.72</td>
      <td>Quelaton80</td>
    </tr>
    <tr>
      <th>779</th>
      <td>23</td>
      <td>Female</td>
      <td>107</td>
      <td>Splitter, Foe Of Subtlety</td>
      <td>3.61</td>
      <td>Alim85</td>
    </tr>
  </tbody>
</table>
<p>780 rows × 6 columns</p>
</div>



players_df = pd.DataFrame(heroes,columns=['Age','SN','Gender','Item ID','Item Name','price'])
players_df.head()


```python
#player count
count_players=len(players_df['SN'].value_counts())
counts_players= pd.DataFrame({"counts_payers":count_players},index=[0])
counts_players
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
      <th>counts_payers</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>573</td>
    </tr>
  </tbody>
</table>
</div>




```python

#Number of Unique Items
unique_items = len(players_df['Item ID'].value_counts())

#Average Purchase Price
average_price = players_df['Price'].mean()

#Total Number of Purchases
total_purchases = players_df['Item Name'].count()


#Total Revenue
total_revenue = players_df['Price'].sum()

#Create DataFrame
purchasing_analysis = pd.DataFrame({"Number of Unique Items": [unique_items],
                                  "Average Price": [average_price],
                                  "Total Purchases": [total_purchases],
                                  "Total Revenue": [total_revenue],
                               
})

purchasing_analysis

```


    ---------------------------------------------------------------------------

    KeyError                                  Traceback (most recent call last)

    /anaconda3/lib/python3.6/site-packages/pandas/core/indexes/base.py in get_loc(self, key, method, tolerance)
       3062             try:
    -> 3063                 return self._engine.get_loc(key)
       3064             except KeyError:


    pandas/_libs/index.pyx in pandas._libs.index.IndexEngine.get_loc()


    pandas/_libs/index.pyx in pandas._libs.index.IndexEngine.get_loc()


    pandas/_libs/hashtable_class_helper.pxi in pandas._libs.hashtable.PyObjectHashTable.get_item()


    pandas/_libs/hashtable_class_helper.pxi in pandas._libs.hashtable.PyObjectHashTable.get_item()


    KeyError: 'Price'

    
    During handling of the above exception, another exception occurred:


    KeyError                                  Traceback (most recent call last)

    <ipython-input-19-abc558fb80bd> in <module>()
          4 
          5 #Average Purchase Price
    ----> 6 average_price = players_df['Price'].mean()
          7 
          8 #Total Number of Purchases


    /anaconda3/lib/python3.6/site-packages/pandas/core/frame.py in __getitem__(self, key)
       2683             return self._getitem_multilevel(key)
       2684         else:
    -> 2685             return self._getitem_column(key)
       2686 
       2687     def _getitem_column(self, key):


    /anaconda3/lib/python3.6/site-packages/pandas/core/frame.py in _getitem_column(self, key)
       2690         # get column
       2691         if self.columns.is_unique:
    -> 2692             return self._get_item_cache(key)
       2693 
       2694         # duplicate columns & possible reduce dimensionality


    /anaconda3/lib/python3.6/site-packages/pandas/core/generic.py in _get_item_cache(self, item)
       2484         res = cache.get(item)
       2485         if res is None:
    -> 2486             values = self._data.get(item)
       2487             res = self._box_item_values(item, values)
       2488             cache[item] = res


    /anaconda3/lib/python3.6/site-packages/pandas/core/internals.py in get(self, item, fastpath)
       4113 
       4114             if not isna(item):
    -> 4115                 loc = self.items.get_loc(item)
       4116             else:
       4117                 indexer = np.arange(len(self.items))[isna(self.items)]


    /anaconda3/lib/python3.6/site-packages/pandas/core/indexes/base.py in get_loc(self, key, method, tolerance)
       3063                 return self._engine.get_loc(key)
       3064             except KeyError:
    -> 3065                 return self._engine.get_loc(self._maybe_cast_indexer(key))
       3066 
       3067         indexer = self.get_indexer([key], method=method, tolerance=tolerance)


    pandas/_libs/index.pyx in pandas._libs.index.IndexEngine.get_loc()


    pandas/_libs/index.pyx in pandas._libs.index.IndexEngine.get_loc()


    pandas/_libs/hashtable_class_helper.pxi in pandas._libs.hashtable.PyObjectHashTable.get_item()


    pandas/_libs/hashtable_class_helper.pxi in pandas._libs.hashtable.PyObjectHashTable.get_item()


    KeyError: 'Price'

