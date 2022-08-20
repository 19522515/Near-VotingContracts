# Near-VotingContracts
https://learnnear.club/near-live-contract-review-part-1-voting-contracts/#Structural_Overview
# Tổng kết kiến thức đạt được:
- Biết xài VMWARE để giả lập ubuntu trên Win10 và cài đặt các công cụ cần thiết
- Biết xuất ra file .wasm và deploy thành công, gọi được các hàm method của smart contract và đọc hiểu
- Tuy không có thay đổi và sửa code nhưng đã hiểu được basic của contract và quản lí cũng như truy cập được nó

# Hướng dẫn:
https://brson.github.io/2020/09/07/near-smart-contracts-rust  -> LINK huong dan build ra file .wasm.
 Sau khi them file package.json va viet code 

{
    "name": "my-package",
    "scripts": {
        "build": "cargo build --target wasm32-unknown-unknown --release",
        "postbuild": "cp target/wasm32-unknown-unknown/release/voting_contract.wasm ./res/",
        "test": "asp"
    },
    "devDependencies": {
        "near-sdk-as": "^3.2.3"
    }
}
  
  -> Va chay lenh   'npm run build'   thi se xuat ra file .wasm o thu muc res
  ( If error thi chay lenh 'rustup target add wasm32-unknown-unknown' truoc)
  Sau do ta chi can chay lenh    'near deploy vietvuive.testnet voting_contract.wasm' la oke 
  ( truoc het phai near login va 'cd res' noi chua file .wasm)
# Bạn cần liện hệ hay giúp đỡ: 
  FB: https://www.facebook.com/viethappy/
  Email: 19522515@gm.uit.edu.vn
