---
title: Dadgum Box Scores
layout: factors
---


# Dadgum Box Scores 

## Four Factors game-by-game 2016-17

#### Not sure what the Four Factors are? Get [help here](https://cbbstatshelp.com/four-factors/intro/).

<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
     <tr style="background-color:#fff">
     <th scope="col" colspan="1"></th>
     <th scope="col" colspan="5">Offense</th>
     <th scope="col" colspan="5">Defense</th>
    </tr>
         <tr> 
          <th data-sortable="false">Box Score</th>
           <th class="larrydrew">eFG% ↑↓</th>
           <th class="larrydrew">TO% ↑↓</th>
           <th class="larrydrew">OR% ↑↓</th>
           <th class="larrydrew">FTRate ↑↓</th>
           <th class="larrydrew">PPP ↑↓</th>
           <th class="larrydrew">eFG% ↑↓</th>
           <th class="larrydrew">TO% ↑↓</th>
           <th class="larrydrew">OR% ↑↓</th>
           <th class="larrydrew">FTRate ↑↓</th>
           <th class="larrydrew">PPP ↑↓</th>
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
        <td class="larrydrew">{{ factor.ppp }}</td>
        <td class="larrydrew">{{ factor.oefg }}</td> 
        <td class="larrydrew">{{ factor.oto }}</td>
        <td class="larrydrew">{{ factor.oor }}</td>
        <td class="larrydrew">{{ factor.oft }}</td>
        <td class="larrydrew">{{ factor.oppp }}</td>
  			</tr>
  			{% endfor %}
    </tbody>
</table>


