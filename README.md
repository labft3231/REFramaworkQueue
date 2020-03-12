# REFramaworkQueue


### - Excel 데이터를 읽어 Queue를 만들고 Queue에서 가져온 데이터로 다른 Excel 파일 만들기


#### 1. init
```
 - Data\Input 폴더의 Input.xlsx 파일의 셀을 read 하여서 Queue로 저장
```

#### 2. GetTransactionData
```
 - Queue에서 데이터 가져오기
 - TransactionNumber 값 보다 데이터 가져온 row수가 작다면 out_Transaction을 out_transaction으로
 - 크다면 out_transaction은 할게 없으니 Nothing으로 바꿔준다.
```

#### 3. Process
```
 - Queue의 데이터를 가져올경우 경우엔 SpecificContent("큐에 저장한 key명")을 활용하여 가져온다.
 - 그런 다음 원하는 작업을 시행하면 된다. 여기서는 가져온 값의 앞자리가 짝수일때 output.xlsx로 저장된다.
```
 
