# PDO-ActiveRecord

實作類似 CodeIgniter 的 Active Record 類別

# How to use
```php

require_once dirname(__FILE__) . '/activeRecord.php';

use Lee\ActiveRecord;

$db = new ActiveRecord();

//Exapmle 1
$query = $db->get('mytable');
// 產生： SELECT * FROM mytable

//Exapmle 2
$query = $db->get_where('mytable', array('id' => $id), $limit, $offset);
// 產生： SELECT * FROM mytable WHERE id = '1' LIMIT 1, 10

```
[更多範例可參考 CI 文件](https://codeigniter.org.tw/user_guide/database/active_record.html)

