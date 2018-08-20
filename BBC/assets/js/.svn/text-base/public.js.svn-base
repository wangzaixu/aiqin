//$.fn.bootstrapDualListbox.defaults={infoText:"共 {0}",infoTextFiltered:'<span class="label label-warning">Filtered</span> {0} from {1}',infoTextEmpty:"Empty list"}
//table全选
$(".table").on("click","thead .tab-selectAll",function(){
	var that=$(this);
	var table=that.closest(".table");
	var slectCheckboxs=table.find("input.table-checkbox[type=checkbox]");
//	var allCheckbox=
	var isCheck=that.eq(0).prop("type")=="checkbox"?that.prop("checked"):that.find("input[type=checkbox]").prop("checked");
	console.log(that);
	console.log(that.eq(0).prop("type"));
	if(isCheck){
//		console.log("全部选中");
		slectCheckboxs.prop("checked",true);
	}else{
//		console.log("全部");
		slectCheckboxs.prop("checked",false);
	}
})
//
$(".table").on("click","tbody input.table-checkbox[type=checkbox]",function(){
	var that=$(this);
	var table=that.closest(".table");
	var row=that.closest("tr");
	var allCheckbox=table.find("input.tab-selectAll[type=checkbox]");
	var alllen=table.find("input.table-checkbox[type=checkbox]").length;
	var slectCheckboxs=table.find("input.table-checkbox[type=checkbox]:checked");
	var checklen=slectCheckboxs.length;
	var isAllCheck=(alllen==checklen);
	var isCheck=that.is(":checked");
	
	if(isCheck){
		row.addClass("selected");
	}else{
		row.removeClass("selected");
	}
	
	if(isAllCheck){
		allCheckbox.prop("checked",true);
	}else{
		allCheckbox.prop("checked",false);
	}
})
