---
title: Dadgum Box Scores
layout: default
---

# Dadgum Box Scores 

## Every UNC Box Score Since 03-04

#### Filter by season, wins, losses, opponent or type of game


<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
         <tr> 
           <th>Season ↑↓</th>
           <th>Date ↑↓</th>
           <th style="display: none;">Result ↑↓</th>
           <th>Location ↑↓</th>
           <th>Type ↑↓</th>
           <th data-sortable="false">Box Score</th>
         </tr>
     </thead>

    <tbody>
	{% for all in site.data.alls %}
		<tr style="background-color: #{{ all.style }};">
  			<td>{{ all.season }}</td> 
  			<td>{{ all.date }}</td> 
  			<td style="display: none;">{{ all.result }}</td>
  			<td>{{ all.location }}</td>
  			<td>{{ all.type }}</td>
  			<td><a href="{{ all.box }}" target="_blank">{{ all.game }}</a></td></tr>
  			{% endfor %}
    </tbody>
</table>


