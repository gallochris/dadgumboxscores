---
title: Dadgum Box Scores
layout: factors
---


# Dadgum Box Scores 

## Four Factors game-by-game 2016-17

<pre class="huffman stilwata">
| When UNC has a . .  | it's record is . . |
|:-------------------:|:------------------:|
|     Higher eFG%     |         21-0       |
|      Lower eFG%     |         12-7       |
|      Higher TO%     |         11-3       |
|      Lower TO%      |         21-4       |
|       Same TO%      |          1-0       |
|      Higher OR%     |         33-3       |
|      Lower OR%      |          0-4       |
|    Higher FTRate    |         24-2       |
|     Lower FTRate    |          9-5       |
</pre>


#### Not sure what the Four Factors are? Get [help here](https://cbbstatshelp.com/four-factors/intro/).

<table id="example" class="display center" cellspacing="0" width="100%" style="table-layout:auto;">
	<thead>
     <tr>
     <th scope="col" colspan="1" class="larrydrew"></th>
     <th scope="col" colspan="4" class="larrydrew">Offense</th>
     <th scope="col" colspan="8" style="padding-left: 450px" class="larrydrew">Defense</th>
    </tr>
         <tr> 
           <th class="larrydrew janet">eFG%</th>
           <th class="larrydrew janet">TO%</th>
           <th class="larrydrew janet">OR%</th>
           <th class="larrydrew janet">FTRate</th>
           <th class="larrydrew janet">PPP</th>
          <th class="huffman" data-sortable="false">Box Score</th>
           <th class="larrydrew janet">eFG%</th>
           <th class="larrydrew janet">TO%</th>
           <th class="larrydrew janet">OR%</th>
           <th class="larrydrew janet">FTRate</th>
           <th class="larrydrew janet">PPP</th>
         </tr>
     </thead>

    <tbody>
	{% for factor in site.data.factors %}
		<tr>
  			<td class="larrydrew janet">{{ factor.efg }}</td> 
  			<td class="larrydrew janet">{{ factor.to }}</td>
  			<td class="larrydrew janet">{{ factor.or }}</td>
  			<td class="larrydrew janet">{{ factor.ft }}</td>
        <td class="larrydrew janet">{{ factor.ppp }}</td>
            <td class="huffman"><span style="background-color:#{{ factor.style }}; padding: 2px 2px;"><a href="{{ factor.box }}" target="_blank">{{ factor.game }}</a></span></td>
        <td class="larrydrew janet">{{ factor.oefg }}</td> 
        <td class="larrydrew janet">{{ factor.oto }}</td>
        <td class="larrydrew janet">{{ factor.oor }}</td>
        <td class="larrydrew janet">{{ factor.oft }}</td>
        <td class="larrydrew janet">{{ factor.oppp }}</td>
  			</tr>
  			{% endfor %}
    </tbody>
</table>


