---
title: Dadgum Box Scores
layout: factors
---


# Dadgum Box Scores 

## Four Factors game-by-game 2016-17

<pre style="text-align: center">
| When UNC has a . .  | it's record is . . |
|:-------------------:|:------------------:|
|     Higher eFG%     |         16-0       |
|      Lower eFG%     |          9-5       |
|      Higher TO%     |          8-2       |
|      Lower TO%      |         16-3       |
|       Same TO%      |          1-0       |
|      Higher OR%     |         25-2       |
|      Lower OR%      |          0-3       |
|    Higher FTRate    |         19-2       |
|     Lower FTRate    |          6-3       |
</pre>


#### Not sure what the Four Factors are? Get [help here](https://cbbstatshelp.com/four-factors/intro/).

<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
     <tr style="background-color:#fff">
     <th scope="col" colspan="1" class="larrydrew"></th>
     <th scope="col" colspan="5" class="larrydrew">Offense</th>
     <th scope="col" colspan="5" class="larrydrew">Defense</th>
    </tr>
         <tr> 
          <th data-sortable="false">Box Score</th>
           <th class="larrydrew">eFG% ↑↓</th>
           <th class="larrydrew">TO% ↑↓</th>
           <th class="larrydrew">OR% ↑↓</th>
           <th class="larrydrew">FTRate ↑↓</th>
           <th>PPP ↑↓</th>
           <th class="larrydrew">eFG% ↑↓</th>
           <th class="larrydrew">TO% ↑↓</th>
           <th class="larrydrew">OR% ↑↓</th>
           <th class="larrydrew">FTRate ↑↓</th>
           <th>PPP ↑↓</th>
         </tr>
     </thead>

    <tbody>
	{% for factor in site.data.factors %}
		<tr style="background-color: #{{ factor.style }};">
    <td><a href="{{ factor.box }}" target="_blank">{{ factor.game }}</a></td>
  			<td class="larrydrew">{{ factor.efg }}</td> 
  			<td class="larrydrew">{{ factor.to }}</td>
  			<td class="larrydrew">{{ factor.or }}</td>
  			<td class="larrydrew">{{ factor.ft }}</td>
        <td>{{ factor.ppp }}</td>
        <td class="larrydrew">{{ factor.oefg }}</td> 
        <td class="larrydrew">{{ factor.oto }}</td>
        <td class="larrydrew">{{ factor.oor }}</td>
        <td class="larrydrew">{{ factor.oft }}</td>
        <td>{{ factor.oppp }}</td>
  			</tr>
  			{% endfor %}
    </tbody>
</table>


