<!-- 
.. title: Mourinho is right about Fàbregas
.. slug: mourinho-is-right-about-fabregas
.. date: 2014-08-24 19:12:19 UTC+01:00
.. tags: football, Mourinho
.. link: 
.. description: 
.. type: text
-->

Mourinho's statement that ["Barcelona misused Cesc Fábregas"](http://www.theguardian.com/football/2014/aug/19/jose-mourinho-cesc-fabregas-chelsea-burnley) has stired some controversy, as expected. One common critique was that Fàbregas is known for having a great start of the season, but loses steam as the season progresses.

But is Mourinho right about Fàbregas capacity to "control the game and dictate the intensity of it" due to the way he is being used at Chelsea?

<!-- TEASER_END -->

I figured using only the first two matches of each season would be a fair comparision. These are all the passes made by Fàbregas in the first two league matches of this and the past season.

![reddit1](/images/fabregas.svg)

Passes made for Chelsea, in blue, are mostly made around the midfield, while Barcelona's passes are made up front. This is clear if we look at stats after dividing the pitch in 5 equal parts:

<table border="1" class="table">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th></th>
      <th>Passes</th>
      <th>Key Passes</th>
      <th>Long Passses</th>
    </tr>
    <tr>
      <th>Team Name</th>
      <th>Fifth</th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th rowspan="5" valign="top">Barcelona</th>
      <th>1</th>
      <td>  1</td>
      <td> 0</td>
      <td>  0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>  3</td>
      <td> 1</td>
      <td>  1</td>
    </tr>
    <tr>
      <th>3</th>
      <td> 30</td>
      <td> 0</td>
      <td>  3</td>
    </tr>
    <tr>
      <th>4</th>
      <td> 40</td>
      <td> 1</td>
      <td>  2</td>
    </tr>
    <tr>
      <th>5</th>
      <td> 12</td>
      <td> 4</td>
      <td>  0</td>
    </tr>
    <tr>
      <th rowspan="5" valign="top">Chelsea</th>
      <th>1</th>
      <td>  4</td>
      <td> 0</td>
      <td>  1</td>
    </tr>
    <tr>
      <th>2</th>
      <td> 37</td>
      <td> 0</td>
      <td>  5</td>
    </tr>
    <tr>
      <th>3</th>
      <td> 69</td>
      <td> 1</td>
      <td> 15</td>
    </tr>
    <tr>
      <th>4</th>
      <td> 49</td>
      <td> 2</td>
      <td>  1</td>
    </tr>
    <tr>
      <th>5</th>
      <td>  7</td>
      <td> 2</td>
      <td>  0</td>
    </tr>
  </tbody>
</table>

Notice the amount of long passes Fàbregas has been able to make for Chelsea, both due to his lower positioning and the difference in playing styles.

He is also much more involved in the match. He made almost double the amount of passes, and had a better success rate. We can also confirm his lower positioning: his vertical coordinate of his passes is considerably lower:

<table border="1" class="table">
  <thead>
    <tr>
      <th></th>
      <th>Passes</th>
      <th colspan="2" halign="left">Vertical Coordinate</th>
      <th>Success (%)</th>
      <th>Key Passes</th>
      <th>Long Passes</th>
    </tr>
    <tr>
      <th></th>
      <th>sum</th>
      <th>mean</th>
      <th>stdev</th>
      <th>mean</th>
      <th>sum</th>
      <th>sum</th>
    </tr>
    <tr>
      <th>Team Name</th>
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
      <th>Barcelona</th>
      <td>  86</td>
      <td> 67.5</td>
      <td> 16.0</td>
      <td> 0.826</td>
      <td> 6</td>
      <td>  6</td>
    </tr>
    <tr>
      <th>Chelsea</th>
      <td> 166</td>
      <td> 55.2</td>
      <td> 17.0</td>
      <td> 0.904</td>
      <td> 5</td>
      <td> 22</td>
    </tr>
  </tbody>
</table>

The code used to get this values is shared [here](http://nbviewer.ipython.org/github/rjtavares/football-crunching/blob/master/notebooks/is%20mourinho%20right%20about%20fabregas.ipynb). Unfortunately, the data is owned by Opta so it can't be shared.