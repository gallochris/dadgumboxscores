---
title: Dadgum Box Scores
layout: default
---

# Dadgum Box Scores 

## Every UNC Box Score Since 03-04

#### [16-17 game-by-game four factors breakdown](/four-factors/)

#### Filter by season, wins, losses, opponent or type of game

<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
         <tr> 
           <th>Season ↑↓</th>
           <th class="larrydrew">Date ↑↓</th>
           <th style="display: none;">Result ↑↓</th>
           <th class="larrydrew">Location ↑↓</th>
           <th class="larrydrew">Type ↑↓</th>
           <th data-sortable="false">Box Score</th>
         </tr>
     </thead>

    <tbody>
	{% for all in site.data.alls %}
		<tr style="background-color: #{{ all.style }};">
  			<td>{{ all.season }}</td> 
  			<td class="larrydrew">{{ all.date }}</td> 
  			<td style="display: none;">{{ all.result }}</td>
  			<td class="larrydrew">{{ all.location }}</td>
  			<td class="larrydrew">{{ all.type }}</td>
  			<td><a href="{{ all.box }}" target="_blank">{{ all.game }}</a></td></tr>
  			{% endfor %}
    </tbody>
</table>


