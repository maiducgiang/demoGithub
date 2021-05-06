khi một nhánh hotfix được tạo, sau khi fix xong lỗi thì nó sẽ được merge vào những nhánh nào và lý do vì sao lại cần merge vào những nhánh đó.



Trong gitflow,khi phát hiện lỗi sẽ cần sửa khẩn cấp sẽ tạo 1 nhánh hotfix và khi fix được bug sẽ được merge luôn vào nhánh master để tránh gây ảnh hưởng nhiều tới ứng dụng.
Mỗi một hotfix hoặc 1 bản cập nhật được merge vào nhánh master đều phải có gittag
Sau đó nhánh hotfix sẽ được merge vào các nhánh khác theo thứ tự là: canary => stagging=> develop (để tránh hiện tượng bug trên các phiên bản sắp được merge)
+ canary, stagging: fix lỗi gặp phải ở bản dùng thử cho nội bộ và cho 
một lượng nhỏ người dùng 

+ develop: được merge sau khi đã merge ở các nhánh trên, để đồng bộ và sửa phần bug tại code gốc. Tránh việc bug vẫn tiếp tục 
trong các bản cập nhật mới và xảy ra trên các nhánh thực hiện của các dev.