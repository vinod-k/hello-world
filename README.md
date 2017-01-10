# hello-world
My first repository on GitHub.

I love working on Git.

<script type = "text/javascript">
jQuery(document).ready(function(){

	jQuery(".datasubmit").hide();
	jQuery("select.selectval").change(function()
	{
		var selectedVal = jQuery(this).val();
		var rownumber = jQuery(this).attr("rownumber");
		var rowdatastatus= "rowdatastatus"+rownumber;
		jQuery("#"+rowdatastatus).val(selectedVal);
		var datasubmit = "datasubmit"+rownumber;
		jQuery("#"+datasubmit).show();
		var currentid = "selectedvalue"+rownumber;
		selectedVal = jQuery(".username").text();
		jQuery("#"+currentid).text(selectedVal);
		jQuery(".nameforrow").val(rownumber);
		var rowid="rowid"+rownumber;
		//alert(rowid)
		var rowvalue= "";
		jQuery("#"+rowid+" td").each(function()
		{
			rowvalue +=jQuery(this).text();
			rowvalue +="!!!";
		});
		var rowdata= "rowdata"+rownumber
		jQuery("#"+rowdata).val(rowvalue);
		jQuery.alert("Message here","Title here");
		//alert(rowvalue);
	});
	jQuery(".datasubmit").click(function()
	{		
	});
});
</script>
