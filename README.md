# SimpleAdapter

## 1. Introduction:
SimpleAdapter is an adapter for mapping data to views defined in an XML file. You can specify the data to be packaged in a list as an ArrayList of the mapping progress. Each element in the ArrayList is an instance of a row on the ListView.

SimpleAdapter's syntax: SimpleAdapter(Context context, List<? extends Map<String, ?>>data, int resource, String[] from, int[] to).

* Parameters:
    + context: used to refer to the current class, usually "this" keyword is used. 
    + data: a list of data. Each item in the List corresponds to a row in the list. Maps are used to store data on each row.
    + resource: the resource id used to set the lists in the "Layout" directory.
    + from: an array of data series, or a list of column names in Maps to associate with "ListView" or "GridView".
    + to: an integer array to store the ids of the "View". The label of the column is passed in the "from" parameter.

## 2. History:
SimpleAdapter was introduced in Android Studio in API level 1. SimpleAdapter is included in java.lang.Object -> android.widget.BaseAdapter directories.

## 3. Major methods/attributes:

* int getCount(): count the number of items in the data which are set by this SimpleAdapter.
* View getDropDownView(int position, View convertView, ViewGroup parent): retrieve a View that displays in the drop down popup the data at the specified position in the data set.
    + position: index of the item.
    + convertView: the old view to reuse.
    + parent: the parent that the specific view will be attached to.                                                                   
* Resources.Theme getDropDownViewTheme(): return the value previously set by a call to setDropDownViewTheme() function.
* Filter getFilter(): return a filter to constrain data with a filtering pattern.
* Object getItem(int position): get the data item as well as its position in the data set.
* long getItemId(int position): get the row id associated with the position of the data item in the data set.
* View getView(int position, View convertView, ViewGroup parent): get a view that data is displayed 
