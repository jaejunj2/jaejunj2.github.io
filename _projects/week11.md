---
name: My new homework
tools: [Python, HTML, vega-lite]
image: assets/pngs/my_png.png
description: This is a "showcase" project that uses vega-lite for interactive viz!
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Example including vega-lite

Example comes from this [great blog post right here](https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html) that was also used in [our test import script](https://github.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/blob/main/week01/test_imports_week01.ipynb).

We can use a vegachart HTML tag like so:

```
<vegachart schema-url="{{ site.baseurl }}/assets/json/altair_license.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/altair_license.json" style="width: 100%"></vegachart>

This visualize the distribution of license status based on each state. Also, the audience can choose status of license that they are interested in. The Color is used to show the number of linces status in the specific state. I have used nominal scales since both States and License Status do not have order. On ther other hand, they are just different. Therefore, I chose nominal scale and did not choose ordinal scale. I did not do any transformation for the first plot. The main reason for not using transformation is because both x and y values are nominal data, therefore, I did not think I need any transformation.

This might be interested for people who wanted to do license-related service; since it would be better to run a business in a state with many not renewed licenses.

This visualize the distribution of license status based on each state. Also, the audience can choose status of license that they are interested in. The Color is used to show the number of linces status in the specific state. I have used nominal scales since both States and License Status do not have order. On ther other hand, they are just different. Therefore, I chose nominal scale and did not choose ordinal scale. I did not do any transformation for the first plot. The main reason for not using transformation is because both x and y values are nominal data, therefore, I did not think I need any transformation.

This might be interested for people who wanted to do license-related service; since it would be better to run a business in a state with many not renewed licenses.


```
<vegachart schema-url="{{ site.baseurl }}/assets/json/second_altair_license.json" style="width: 100%"></vegachart>
```

<vegachart schema-url="{{ site.baseurl }}/assets/json/second_altair_license.json" style="width: 100%"></vegachart>


This visualize shows ho the specific license is distributed for multiple states based on year. Different description uses different color. I have created visualization like this so that the audience can see different color when they choose different descriptions, which can improve the audiences' interactive experiment. I have changed the size of circles based on the count number, which can show how the number of specific license changes as the time goes for multiple states. For Description and State, I have used nominal scale, since they are categorical without specific ordrer. However, for year, I have used temporal scale. To improve readability I have only extracted years from original date. It is important to note that the year suggests the year of last modified date. I did not do any formal transformation. However, to ease the process of creating features, I have selected cokumns from original data frame and created smaller data frame. I did this way because it is more straightfoward than using formal transformation.

This might be interested for people who wanted to see how diverse licneses have changed over time.




## Search The Data & Methods

Below is where we can put some links to both the data and the analysis code as buttons:

```
<div class="left">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/licenses_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://blog.4dcu.be/programming/2021/05/03/Interactive-Visualizations.html" text="The Analysis" %}
</div>
```

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/UIUC-iSchool-DataViz/is445_data/raw/main/licenses_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="my_Workbook.ipynb" text="The Analysis" %}
</div>