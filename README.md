## Angular(2+) Table with search

In angular 2 we don't have pre-defined filter and order by as it was with AngularJs, we need to create it for our requirements. It is time killing but we need to do it, (No FilterPipe). Here, we are going to see how we can create filter in angular 2.

Through this project, you will learn using Angular(2+) :

- how you can create a dynamic table. 
- how you can implement a search bar to filter the content of table.

## Example:
```
<th><input type="text" name="name" [(ngModel)]="filter.name" placeholder="name"></th>
<th><input type="text" name="city" [(ngModel)]="filter.city" placeholder="city"></th>

<tr *ngFor="let user of userDetails | userfilter:filter"> 
  <td>{{user.name}}</td>
  <td>{{user.city}}</td>
</tr>
```
