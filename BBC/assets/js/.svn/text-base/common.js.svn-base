$(function(){
	//.full-check  全选 复选框
	//.one-check   单个 复选框
	//.table 	      此table针对ace中表格
	
	//全选
	    $('.full-check').on('click',function(){   
		    if(this.checked){   
		        $('.table .one-check').prop("checked", true);  
		    }else{   
			$(".table .one-check").prop("checked", false);
		    }   
		});
		
	//判断全选状态
		$('.table .one-check').on('click',function(){
			var $this = $(this),
				$tableNode = $this.parents('.table'),
				$oneCheck = $tableNode.find('.one-check'),
				
				$dynamicTable = $this.parents('.dataTables_wrapper'),
				$dynamicfullCheck = $dynamicTable.find('.full-check'),
				
				chknum = $oneCheck.size(),//选项总个数
				chk = 0;
				
				console.log(chknum);
				$oneCheck.each(function () {  
		        if($(this).prop("checked")==true){
						chk++;
					}
			    });
			    
				if(chknum==chk){  //全选
					$dynamicfullCheck.prop("checked",true);
				}else{ //不全选
					$dynamicfullCheck.prop("checked",false);
				}
		});
});

//layer默认配置
	if(layer)
	layer.config({
		btnAlign: 'c',		//按钮居中
		shadeClose:true,	//开启弹层关闭
		scrollbar: true,	//不允许浏览器滚动
		resize:false		//不允许拉伸
	});
	
	
