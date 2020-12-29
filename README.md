# Blood-pressure-kotlin-App-
Blood pressure app displays the patients blood pressure to the user based on their input or hardcoded data .
 It is a list of Blood Pressure readings. 
 This is done by adding a RecyclerView, Adapter and a View Holder. The adaptor class tells the RecyclerView how to display each item( in this case the readings).
 Adapter For Recycler View11The Adapter needs three methods: 1.onCreateViewHolder() 2.getItemCount() 3.onBindViewHolder()
The RecyclerView first calls getItemCount()for the number of items in the list.
It then loops or each item, as needed:
1.If a new ViewHolder is needed, it calls onCreateViewHolder() otherwise it recycles an existing one.
2.It then calls onBinViewHolder with the item number.
3.The adapter looks up the item number in the list and populates its fields with the item data.
 You also would need to create a navaigation graph, you dp this by adding a NavHostFragment to the main Activity
*Click on MainActivity’s layout file, activity_main.xml, in the res layout folder.
Delete the TextView from the layout.
In the Palette panel, select the Container group and drag a NavHostFragment into the ConstraintLayout.
Click OK to select the navigation graph we created, the only one in the app.
Give the NavHostFragment the id “nav_host_fragment”.*
