# Size Guide - Example Body Content

## How to Add This Content to Your Metaobject

### Step 1: Go to Your Metaobject
1. Shopify Admin → **Settings** → **Custom data** → **Metaobjects**
2. Click on your `size_guide` type
3. Click on your size guide entry (or create a new one)

### Step 2: Fill in the Fields

**Title Field:**
```
Classic Running Shoes Size Guide
```

**Body Field (Rich Text):**

Use the rich text editor in Shopify to create a table. Here's what to enter:

---

## Option 1: Using Shopify's Rich Text Editor

1. Click in the **Body** field
2. Click the **Table** icon in the toolbar
3. Create a table with **5 columns** and **8 rows** (1 header + 7 data rows)
4. Fill in the table as follows:

### Table Content:

**Header Row:**
| UK/IN | US | EURO | To Fit Foot Length (in) | To Fit Foot Length (cm) |

**Data Rows:**
| 6 | 7 | 40 | 9.84 | 25 |
| 7 | 8 | 41 | 10.24 | 26 |
| 8 | 9 | 42 | 10.63 | 27 |
| 9 | 10 | 43 | 11.02 | 28 |
| 10 | 11 | 44 | 11.42 | 29 |
| 11 | 12 | 45 | 11.81 | 30 |
| 12 | 13 | 46 | 12.20 | 31 |

---

## Option 2: If Rich Text Editor Doesn't Support Tables

If Shopify's rich text editor doesn't have a table option, you can use **HTML** instead. Change the field type to **Multi-line text** and paste this HTML:

```html
<h2>MEN'S FOOTWEAR</h2>

<table>
  <thead>
    <tr>
      <th>UK/IN</th>
      <th>US</th>
      <th>EURO</th>
      <th>To Fit Foot Length (in)</th>
      <th>To Fit Foot Length (cm)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>6</td>
      <td>7</td>
      <td>40</td>
      <td>9.84</td>
      <td>25</td>
    </tr>
    <tr>
      <td>7</td>
      <td>8</td>
      <td>41</td>
      <td>10.24</td>
      <td>26</td>
    </tr>
    <tr>
      <td>8</td>
      <td>9</td>
      <td>42</td>
      <td>10.63</td>
      <td>27</td>
    </tr>
    <tr>
      <td>9</td>
      <td>10</td>
      <td>43</td>
      <td>11.02</td>
      <td>28</td>
    </tr>
    <tr>
      <td>10</td>
      <td>11</td>
      <td>44</td>
      <td>11.42</td>
      <td>29</td>
    </tr>
    <tr>
      <td>11</td>
      <td>12</td>
      <td>45</td>
      <td>11.81</td>
      <td>30</td>
    </tr>
    <tr>
      <td>12</td>
      <td>13</td>
      <td>46</td>
      <td>12.20</td>
      <td>31</td>
    </tr>
  </tbody>
</table>

<h3>How to Measure Your Foot</h3>
<p>Place your foot on a piece of paper and mark the heel and longest toe. Measure the distance between the two marks.</p>

<h3>Size Tips</h3>
<ul>
  <li>If you're between sizes, we recommend sizing up</li>
  <li>Measure your feet at the end of the day when they're largest</li>
  <li>Wear the socks you plan to wear with the shoes</li>
</ul>
```

---

## Option 3: Complete Example with Multiple Sections

Here's a more comprehensive example with additional helpful information:

```html
<h2>MEN'S FOOTWEAR SIZE GUIDE</h2>

<table>
  <thead>
    <tr>
      <th>UK/IN</th>
      <th>US</th>
      <th>EURO</th>
      <th>To Fit Foot Length (in)</th>
      <th>To Fit Foot Length (cm)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>6</td>
      <td>7</td>
      <td>40</td>
      <td>9.84</td>
      <td>25</td>
    </tr>
    <tr>
      <td>7</td>
      <td>8</td>
      <td>41</td>
      <td>10.24</td>
      <td>26</td>
    </tr>
    <tr>
      <td>8</td>
      <td>9</td>
      <td>42</td>
      <td>10.63</td>
      <td>27</td>
    </tr>
    <tr>
      <td>9</td>
      <td>10</td>
      <td>43</td>
      <td>11.02</td>
      <td>28</td>
    </tr>
    <tr>
      <td>10</td>
      <td>11</td>
      <td>44</td>
      <td>11.42</td>
      <td>29</td>
    </tr>
    <tr>
      <td>11</td>
      <td>12</td>
      <td>45</td>
      <td>11.81</td>
      <td>30</td>
    </tr>
    <tr>
      <td>12</td>
      <td>13</td>
      <td>46</td>
      <td>12.20</td>
      <td>31</td>
    </tr>
  </tbody>
</table>

<h3>WOMEN'S FOOTWEAR SIZE GUIDE</h3>

<table>
  <thead>
    <tr>
      <th>UK</th>
      <th>US</th>
      <th>EURO</th>
      <th>To Fit Foot Length (in)</th>
      <th>To Fit Foot Length (cm)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>3</td>
      <td>5</td>
      <td>36</td>
      <td>8.86</td>
      <td>22.5</td>
    </tr>
    <tr>
      <td>4</td>
      <td>6</td>
      <td>37</td>
      <td>9.25</td>
      <td>23.5</td>
    </tr>
    <tr>
      <td>5</td>
      <td>7</td>
      <td>38</td>
      <td>9.65</td>
      <td>24.5</td>
    </tr>
    <tr>
      <td>6</td>
      <td>8</td>
      <td>39</td>
      <td>10.04</td>
      <td>25.5</td>
    </tr>
    <tr>
      <td>7</td>
      <td>9</td>
      <td>40</td>
      <td>10.43</td>
      <td>26.5</td>
    </tr>
    <tr>
      <td>8</td>
      <td>10</td>
      <td>41</td>
      <td>10.83</td>
      <td>27.5</td>
    </tr>
  </tbody>
</table>

<h3>How to Measure Your Foot</h3>
<ol>
  <li>Place a piece of paper on a hard floor against a wall</li>
  <li>Stand on the paper with your heel against the wall</li>
  <li>Mark the longest part of your foot on the paper</li>
  <li>Measure the distance from the wall to the mark</li>
  <li>Use the measurement to find your size in the chart above</li>
</ol>

<h3>Fitting Tips</h3>
<ul>
  <li>If you're between sizes, we recommend choosing the larger size</li>
  <li>Measure your feet at the end of the day when they're at their largest</li>
  <li>Wear the type of socks you plan to wear with the shoes</li>
  <li>Leave about 0.5 inches (1.3 cm) between your longest toe and the end of the shoe</li>
</ul>

<h3>Still Not Sure?</h3>
<p>Contact our customer service team for personalized sizing assistance. We're here to help you find the perfect fit!</p>
```

---

## Quick Copy-Paste Version (Minimal)

Just want the men's footwear table? Copy this:

```html
<table>
  <thead>
    <tr>
      <th>UK/IN</th>
      <th>US</th>
      <th>EURO</th>
      <th>To Fit Foot Length (in)</th>
      <th>To Fit Foot Length (cm)</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>6</td><td>7</td><td>40</td><td>9.84</td><td>25</td></tr>
    <tr><td>7</td><td>8</td><td>41</td><td>10.24</td><td>26</td></tr>
    <tr><td>8</td><td>9</td><td>42</td><td>10.63</td><td>27</td></tr>
    <tr><td>9</td><td>10</td><td>43</td><td>11.02</td><td>28</td></tr>
    <tr><td>10</td><td>11</td><td>44</td><td>11.42</td><td>29</td></tr>
    <tr><td>11</td><td>12</td><td>45</td><td>11.81</td><td>30</td></tr>
    <tr><td>12</td><td>13</td><td>46</td><td>12.20</td><td>31</td></tr>
  </tbody>
</table>
```

---

## Important Notes

1. **Field Type**: Make sure the "body" field in your metaobject definition is set to **"Multi-line text"** if you're pasting HTML directly.

2. **If Using Rich Text**: If your field is "Rich text", use the visual table editor in Shopify instead of pasting HTML.

3. **Save Changes**: Don't forget to click **Save** after adding the content!

4. **Refresh Your Store**: After saving, refresh your product page to see the changes.

---

## Expected Result

When you click the "Size Guide" button, you should see:
- A clean, professional table
- Centered text
- Alternating row colors (subtle gray)
- Hover effects on rows
- Bold header row
- Mobile-responsive layout

The table will look exactly like the reference image you showed me! ✨
