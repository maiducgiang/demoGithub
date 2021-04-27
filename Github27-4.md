1: Khi merge cần có commit, vậy commit merge này có được log trên nhánh được merge vào không (nhánh đích: branch A)?
2: Khi checkout branch B từ branch A, khi mà branch A có commit 1, sau đó 1 thơi gian branch A có 2 commit 
(commit 1 - commit 2), branch B có 3 commit (commit 1 - commit 3 - commit 4), thế nếu merge B vào A xong. Git log ở A,
 thứ tự xuất hiện các commit có phụ thuộc vào thời gian commit của commit 2, 3, 4 không?

Trả lời:

1. Khi merge cần có commit, vậy commit merge này được log trên nhánh đích: branch A.
vì lệnh merge này được thực hiện trên nhánh đích
2. Sau khi thực hiện các thao tác, git log ở A, thứ tự xuất hiện các commit theo thời gian commit của commit 2, 3, 4.

Vậy: Giả sử branchA có lịch sử commit có mã commit: 1 - 2. BranchB được checkout từ branchA tại commit có mã commit là 1 và có lịch sử commit của branchB : 1 - 3 - 4. 
Khi merge branchB vào branchA bằng 2 lệnh "git checkout branchA" và "git merge branchB" 
thì lịch sử commit của branchA có mã commit là: 1 - 2 - 3 - 4 - merge commit.