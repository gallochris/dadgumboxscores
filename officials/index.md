---
title: Dadgum Box Scores | Officials
layout: refs
---

# Dadgum Box Scores 

## Officials game-by-game 2016-17

#### Filter by a referee's first or last name


<pre style="text-align: center">
Most Frequent Officials
|      Name     |  # of Games |
|:-------------:|:-----------:|
 |   Ron Groover |      8      | 
|  Mike Eades   |      7      |
| Ted Valentine |      6      |
</pre>


<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
         <tr> 
           <th data-sortable="false">Box Score</th>
           <th class="larrydrew">Location ↑↓</th>
           <th style="display: none;">Rating ↑↓</th>
           <th data-sortable="false">Ref 1</th>
           <th data-sortable="false">Ref 2</th>
           <th data-sortable="false">Ref 3</th>
         </tr>
     </thead>

    <tbody>
	{% for off in site.data.offs %}
		<tr style="background-color: #{{ off.style }};">
  			<td><a href="{{ off.box }}" target="_blank">{{ off.game }}</a></td>
  			<td class="larrydrew">{{ off.location }}</td> 
        <td style="display: none;">{{ off.rtg }}</td> 
        <td>{{ off.off1 }}</td> 
  			<td>{{ off.off2 }}</td>
  			<td>{{ off.off3 }}</td>
        </tr>
  			{% endfor %}
    </tbody>
</table>


