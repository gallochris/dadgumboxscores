---
title: Dadgum Box Scores | Officials
layout: refs
---

# Dadgum Box Scores 

## Officials game-by-game 2016-17

#### Filter by a referee's first or last name

<table id="example" class="display center" cellspacing="0" width="100%">
	<thead>
         <tr> 
           <th data-sortable="false">Box Score</th>
           <th data-sortable="false">Referee 1</th>
           <th data-sortable="false">Referee 2</th>
           <th data-sortable="false">Referee 3</th>
         </tr>
     </thead>

    <tbody>
	{% for ref in site.data.refs %}
		<tr style="background-color: #{{ ref.style }};">
  			<td><a href="{{ ref.box }}" target="_blank">{{ ref.game }}</a></td>
  			<td>{{ ref.off1 }}</td> 
  			<td>{{ ref.off2 }}</td>
  			<td>{{ ref.off3 }}</td>
        </tr>
  			{% endfor %}
    </tbody>
</table>


