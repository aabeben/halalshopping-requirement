
application/config/constants.php:
  22:         define('API_DATA', 'https://halalshoppingapi.mykisel.com/dev/v1/');
  34:         define('API_DATA', 'https://halalshoppingapi.mykisel.com/staging/v1/');
  45:         define('API_DATA', 'https://halalshoppingapi.mykisel.com/v1/');

application/modules/Cart/controllers/Cart_backup.php:
   98:                 'link' => API_DATA . 'Customers/' . $this->customerId . '/cart?access_token=' . $this->session->userdata('token'),
  381:             'link' => API_DATA . 'escrow/accounts?lastUpdated',
  507:             'link' => API_DATA . 'Customers/' . $this->customerId . '/invoice?access_token=' . $this->session->userdata('token') . '&invoiceId=' . $invoiceId . '',

application/modules/Cart/controllers/Cart.php:
    98:                 'link' => API_DATA . 'Customers/' . $this->customerId . '/cart?access_token=' . $this->session->userdata('token'),
   366:             'link' => API_DATA . 'escrow/accounts?lastUpdated',
   473:             'link' => API_DATA . 'Customers/' . $this->customerId . '/order?access_token=' . $this->session->userdata('token') . '&orderId=' . $orderId . '&lastUpdated',
   682:             'link' => API_DATA . 'Customers/' . $this->customerId . '/invoice?access_token=' . $this->session->userdata('token') . '&invoiceId=' . $invoiceId . '&sort=status&sortItems=status',
   893:             'link' => API_DATA . 'Customers/' . $this->customerId . '/order?access_token=' . $this->session->userdata('token') . '&orderId=' . $orderId,
  1024:             'link' => API_DATA . 'Customers/' . $this->customerId . '/order?access_token=' . $this->session->userdata('token') . '&orderId=' . $orderId,
  1240:             'link' => API_DATA . 'Customers/' . $this->customerId . '/order/delivered?access_token=' . $this->session->userdata('token') . '&orderId=' . $orderId,
  1269:             'link' => API_DATA . 'Customers/' . $this->customerId . '/order?access_token=' . $this->session->userdata('token') . '&orderId=' . $orderId . '',
  1398:             'link' => API_DATA . 'Customers/order/trace?access_token=' . $this->session->userdata('token') . '&orderId=' . str_replace(' ', '', $orderId) . '&id=' . $this->customerId . '',

application/modules/Cart/controllers/Cart(backup - stock checkout issues).php:
  358:             'link' => API_DATA . 'api/escrow/accounts?lastUpdated',

application/modules/Cart/controllers/Checkout.php:
   59:             'link' => API_DATA . 'Customers/' . $this->customerId . '/cart/bulk?access_token=' . $this->session->userdata('token'),
   91:             'link' => API_DATA . 'Couriers?lastUpdated=',
  124:             'link' => API_DATA . 'Customers/' . $this->customerId . '/cart/checkout?access_token=' . $this->session->userdata('token'),
  227:                     'link' => API_DATA . 'Customers/' . $this->customerId . '/pay/bank-transfer?access_token=' . $this->session->userdata('token'),
  472:             'link' => API_DATA . 'Customers/' . $this->customerId . '/cart/shipping-cost?courierId=' . $_POST['courierId'] . '&courierPackageId=' . $_POST['courierPackageId'] . '&shippingAddressId=' . $_POST['shippingAddressId'] . '&access_token=' . $this->session->userdata('token'),
  490:             'link' => API_DATA . 'Customers/' . $this->customerId . '/invoice/validate-voucher?access_token=' . $this->session->userdata('token') . '&voucherCode=' . $voucherCode . '&invoiceId=' . $invoiceId,

application/modules/Cart/models/Cart_model.php:
  97:             'link'   => API_DATA . 'Customers/'.$user->id.'/'.'complaint?access_token='.$this->session->userdata('token'),

application/modules/Cart/models/Checkout_model.php:
   14:             'link' => API_DATA . 'Customers/' . $customerId . '/cart/detail?access_token=' . $this->session->userdata('token') . '&isGift=false',
   28:             'link' => API_DATA . 'Customers/'.$customerId.'/address?skip=&limit=&access_token='.$this->session->userdata('token'),
   94:             'link' => API_DATA . 'Customers/'.$customerId.'/reviews?productId&orderId&type=all&skip&limit&order&lastUpdated=&access_token='.$this->session->userdata('token'),
  370:             'link' => API_DATA . 'Customers/' . $this->customerId . '/invoice?access_token=' . $this->session->userdata('token') . '&invoiceId='.$InvoiceId,
  388:             'link' => API_DATA . 'Customers/'.$customerId.'/pay/bank-transfer?access_token='.$this->session->userdata('token').'',
  409:             'link' => API_DATA . 'Customers/'.$customerId.'/orders?startDate=&endDate=&status=&limit=&skip=&order=&lastUpdated=&access_token='.$this->session->userdata('token'),
  421:             'link' => API_DATA . 'Customers/'.$customerId.'/invoices?access_token='.$this->session->userdata('token').'&lastUpdated=',

application/modules/Cart/views/payment_method_view.php:
  239:     var api = '<?php echo API_DATA; ?>';

application/modules/Cart/views/unggah_bukti_view.php:
  154:                 "url" : "<?php echo API_DATA ?>Customers/<?php echo $this->session->userdata('user')->id ?>/pay/bank-transfer/confirm?access_token=<?php echo $this->session->userdata('token') ?>&invoiceId=<?php echo $invoiceId; ?>",

application/modules/Login/controllers/Login.php:
   71:                 'link' => API_DATA . 'Customers/login',
  148:                 'link' => API_DATA . 'Customers/login',
  217:             'link' => API_DATA . 'Users/reset',

application/modules/Pesan/controllers/Komplain.php:
  70:             'link'   => API_DATA . 'Customers/'.$this->customerId.'/complaint?access_token='.$this->session->userdata('token').'&complaintId='.$this->input->get('tiket').'&limit&skip=&order&lastUpdated=1495477678108',
  92:             'link'   => API_DATA . 'Customers/'.$this->customerId.'/complaint/reply?access_token='.$this->session->userdata('token').'&complaintId='.$this->input->post('Id'),

application/modules/PPOB/controllers/PPOB.php:
   77:             'link' => API_DATA . 'ppob/categories/providers?categoryId=' . $categoryId,
   89:             'link' => API_DATA . 'ppob/products?categoryId=' . $categoryId . '&providerId=' . $providerId . '&skip=&limit=&sortBy=&sortArrangement=',
  163:             'link' => API_DATA . 'escrow/accounts?lastUpdated',
  235:             'link' => API_DATA . 'ppob/orders/voucher:validate?access_token=' . $this->session->userdata('token') . '&customerId=' . $this->customerId . '&orderId=' . $orderId . '&voucherCode=' . $voucherCode,

application/modules/PPOB/models/PPOB_model.php:
   12:                 'link' => API_DATA . 'ppob/categories/products?id=6371781566154276865',
   23:                 'link' => API_DATA . 'ppob/categories/products?id=6429546220208914432',
   34:                 'link' => API_DATA . 'ppob/orders/checkout?access_token='.$this->session->userdata('token').'',
   45:                 'link' => API_DATA . 'ppob/orders/payment/escrow:request?access_token='.$this->session->userdata('token'),
   56:                 'link' => API_DATA . 'ppob/orders/payment/escrow:request?access_token='.$this->session->userdata('token'),
   67:                 'link' => API_DATA . 'ppob/orders/'.$_POST['orderId'].'/pay/tcash?access_token='.$this->session->userdata('token').'',
   78:                 'link' => API_DATA . 'ppob/orders?access_token='.$this->session->userdata('token').'&customerId='.$this->customerId.'',
   89:                 'link' => API_DATA . '/ppob/orders/'.$orderId.'?accessToken='.$this->session->userdata('token').'',
  134:             'link' => API_DATA.'ppob/categories',

application/modules/PPOB/views/payment_method_view.php:
  190:     var api = '<?php echo API_DATA; ?>';

application/modules/PPOB/views/unggah_bukti_view.php:
  151:                 "url" : "<?php echo API_DATA ?>ppob/orders/payment/escrow/proof?access_token=<?php echo $this->session->userdata('token') ?>",
  179:               "url": "<?php echo API_DATA ?>ppob/orders/payment/escrow/confirm?access_token=<?php echo $this->session->userdata('token') ?>",

application/modules/Product/controllers/Product.php:
   93:             $link = API_DATA . 'Products?name=' . urlencode($params['keyword']) . '&categoryId=' . $params['kategori'] . '&merchantId=' . $params['merchant'] . '&merchantCity=' . urlencode($params['location']) . '&ratings=' . $params['rating'] . '&priceRange=' . $price[0] . '|' . $price[1] . '&limit=6&skip=' . $params['skip'] . '&order=' . urlencode($params['sort']) . '&lastUpdated=';
   94:             $linkMeta = API_DATA . 'Products/meta?name=' . urlencode($params['keyword']) . '&categoryId=' . $params['kategori'] . '&merchantId=' . $params['merchant'] . '&merchantCity=' . urlencode($params['location']) . '&ratings=' . $params['rating'] . '&priceRange=' . $price[0] . '|' . $price[1];
   96:             $link = API_DATA . 'Products?name=' . urlencode($params['keyword']) . '&categoryId=' . $params['kategori'] . '&merchantId=' . $params['merchant'] . '&merchantCity=' . urlencode($params['location']) . '&ratings=' . $params['rating'] . '&limit=6&skip=' . $params['skip'] . '&order=' . urlencode($params['sort']) . '&lastUpdated=';
   97:             $linkMeta = API_DATA . 'Products/meta?name=' . urlencode($params['keyword']) . '&categoryId=' . $params['kategori'] . '&merchantId=' . $params['merchant'] . '&merchantCity=' . urlencode($params['location']) . '&ratings=' . $params['rating'] . '&priceRange=';
  205:             'link' => API_DATA . 'Customers/' . $this->customerId . '/product/' . $productId . '/discuss?access_token=' . $this->session->userdata('token'),
  226:             'link' => API_DATA . 'Customers/' . $this->customerId . '/product/discuss/reply?access_token=' . $this->session->userdata('token'),

application/modules/Profile/controllers/Profile.php:
   90:             'link'   => API_DATA . 'Customers/' . $this->customerId . '/address/' . $id . '?access_token=' . $this->session->userdata('token'),
  107:             'link'   => API_DATA . 'Customers/' . $this->customerId . '/profile?access_token=' . $this->session->userdata('token'),
  139:             'link'   => API_DATA . 'Customers/' . $this->session->userdata('user')->id . '/address/' . $id . '?access_token=' . $this->session->userdata('token'),
  185:                 'link'   => API_DATA . 'Customers/' . $this->customerId . '/bank-account/' . $bankAccountId . '?access_token=' . $this->session->userdata('token'),
  203:                 'link'   => API_DATA . 'Customers/' . $this->customerId . '/bank-account?access_token=' . $this->session->userdata('token'),
  222:             'link'   => API_DATA . 'Customers/' . $this->customerId . '/bank-accounts?limit=&skip=&order=&lastUpdated=&access_token=' . $this->session->userdata('token'),
  259:             'link'   => API_DATA . 'Customers/' . $this->customerId . '/address?skip=&limit=&access_token=' . $this->session->userdata('token'),
  311:             'link'   => API_DATA . 'Customers/' . $this->session->userdata('user')->id . '/address?access_token=' . $this->session->userdata('token'),

application/modules/Profile/models/Profile_model.php:
  31:             'link'   => API_DATA . 'Customers/'.$this->customerId.'/profile?access_token='.$this->session->userdata('token'),

application/modules/Profile/views/profile_view.php:
  157:             url: "<?php echo API_DATA ?>Customers/<?php if(!is_null($this->session->userdata('user')->id)) {echo $this->session->userdata('user')->id;} ?>/avatar?access_token=<?php if(!is_null($this->session->userdata('token'))) {echo $this->session->userdata('token'); } ?>",

application/modules/Register/controllers/Register.php:
  76: 	//                'link'   => API_DATA . 'Customers/login',

application/modules/Register/views/register_view.php:
   40:                     url = "<?php echo API_DATA . 'Merchants/register' ?>";
  114:                     url = "<?php echo API_DATA ?>Customers/register";

application/modules/Section/models/Section_model.php:
  167:             'link'   => API_DATA . 'Customers/' . $this->customerId . '/profile?access_token=' . $this->session->userdata('token'),
  309:             'link'   => API_DATA . 'Customers/' . $customerId . '/address?skip=&limit=&access_token=jT6SG2tOOlXZ2GE3JswiAzHCB7Uxr2XgNyMXyChDYrwV3SqF1n6iD4ZrwauGPwZP',
  438:             'link' => API_DATA . 'ppob/categories',

application/modules/templates/controllers/References.php:
  82:                 'link' => API_DATA . 'ppob/products?categoryId=&providerId='.$providerId.'&skip=&limit=&sortBy=&sortArrangement=',
  96:                 'link' => API_DATA . 'ppob/categories/providers?categoryId='.$categoryProduct.'',

application/modules/templates/models/Templates_model.php:
   28:             'link' => API_DATA . 'Customers/' . $this->customerId . '/cart?access_token=' . $this->session->userdata('token') . '&limit&skip&lastUpdated=',
  156:             'link'   => API_DATA . 'Products/categories?name=&limit=&skip=&order=&lastUpdated=&output=tree',
  172:             'link'   => API_DATA . 'Products/categories?name=&skip=&order=&lastUpdated=&output=tree',
  224:             'link'   => API_DATA . 'Customers/' . $this->customerId . '/cart?access_token=' . $this->session->userdata('token') . '&limit&skip&lastUpdated=',

application/modules/templates/views/plugin.php:
  487:             url: '<?php echo API_DATA . 'Customers/'.$this->session->userdata('user')->id.'/order/delivered?access_token='.$this->session->userdata('token').'&orderId='; ?>'+orderId,
  544:             url: '<?php echo API_DATA.'Customers/'.$sess_user_id.'/order/success?access_token='.$sess_token.'&orderId='; ?>'+$idOrder,
