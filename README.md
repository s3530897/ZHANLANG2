# ZHANLANG2 
fuck u;
File file=new File(Environment.getExternalStorageDirectory(),"file2.txt");
        //文件是否存在
        if(!file.exists())
        {
            try {
                //文件不存在，就创建一个新文件
                file.createNewFile();
                System.out.println("文件已经创建了");
            } catch (IOException e) {
                e.printStackTrace();
            }
        }
        else
        {
            System.out.println("文件已经存在");
            System.out.println("文件名："+file.getName());
            System.out.println("文件绝对路径为："+file.getAbsolutePath());
            //是存在工程目录下，所以
            System.out.println("文件相对路径为："+file.getPath());
            System.out.println("文件大小为："+file.length()+"字节");
            System.out.println("文件是否可读："+file.canRead());
            System.out.println("文件是否可写："+file.canWrite());
            System.out.println("我呢间是否隐藏："+file.isHidden());
        }
