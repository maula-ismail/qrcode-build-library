QRcode Build Library
===================

基於 CodeIgniter 的 QRcode 生成程式庫

The QRcode Build library for CodeIgniter

安裝 Installation
=================

複製所有的檔案到 CodeIgniter 根目錄底下。  
Copy all file to the CodeIgniter root path.

使用 Usage
==========

	$this->qrcode->clear()

重設參數

	$this->qrcode->set_file_path(string $dir)

設定 QRcode 生成的檔案存放路徑

	$this->qrcode->set_data(string $data)

設定 QRcode 的內容

	$this->html->set_error_correct(integer $error_correct)

設定 QRcode 的容錯率 預設為 L  
L(7%), M(15%), Q(25%), H(30%)

	$this->html->set_module_size(integer $module_size)

設定單一點的大小(px) 預設為 4

	$this->html->set_point_color(string $color[, string $color1, string $color2])

設定點的顏色(px) 預設為 000000 (黑色)  
輸入一個參數，則顏色採用 RGB 16進位 文字表示，不用加 # 字號  
輸入三個參數，則顏色採用 RGB 10進位 數字，每一個參數代表一個顏色

	$this->html->set_background_color(string $color[, string $color1, string $color2])

設定背景的顏色(px) 預設為 FFFFFF (白色)  
輸入一個參數，則顏色採用 RGB 16進位 文字表示，不用加 # 字號  
輸入三個參數，則顏色採用 RGB 10進位 數字，每一個參數代表一個顏色

	$this->html->set_version(integer $version)

設定 QRcode 使用的圖像版本  
數字 0 ~ 40, 0 表示自動選擇合適的版本

	$this->html->build([string $file_name])

設定檔名並生成圖片，如不設定檔名將自動亂碼命名  
回傳 圖片的檔名

感謝 Thank
==========

本成是使用的 QRCode 圖像轉換程式源自於 http://www.swetake.com/qrcode/qr_cgi_e.html