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

	$this->html->set_version(integer $version)

設定 QRcode 使用的圖像版本  
數字 0 ~ 40, 0 表示自動選擇合適的版本

	$this->html->build([string $file_name])

設定檔名並升成圖片，如不設定檔名將自動亂碼命名
回傳 圖片的檔名