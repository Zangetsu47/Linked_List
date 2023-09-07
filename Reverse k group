void reverseKGroup(int k) {
	        List<Integer>list=new LinkedList<>();
			List<Integer>res=new LinkedList<>();
	        Node current=head;
	        while(current!=null)
	        {
	            list.add(current.data);
	            current=current.next;
	        }
			int num1=list.size()%k;
			int num2=list.size()/k;
			for(int i=0;i<num1;i++)
			{
				list.add(-1);
			}
			for(int i=0;i<list.size()-k+1;i+=k)
			{
				List<Integer>temp=new LinkedList<>();
				for(int j=i;j<i+k;j++)
				{
					temp.add(list.get(j));
				}
				Collections.reverse(temp);
				System.out.println(temp);
				for(Integer e:temp)
				{
					if(e!=-1)
						res.add(e);
				}
			}
			System.out.println(res);
	        current=head;
	        int index=0;
	        while(current!=null)
	        {
	        		current.data=res.get(index++);
	            current=current.next;
	            if(index==k*num2)
	            	break;
	        }
	    }
