
<img width="50%" src="./../images/unafeed_logo.png"/>
<br><br>
<img width="50%" src="./../images/garuda_logo2.png"/>

# Unafeed Backend

### *__Specifications__*

Created using ```node.js``` (```express.js```) and some dependencies:

```json
"cors": "^2.8.5",
"express": "^4.17.1",
"express-fileupload": "^1.2.0",
"mysql": "^2.18.1"
```

<hr>

### *__API lists__*

- __Users__

    ```bash
    GET /user

    GET /user/{ uid }

    POST /signup 
    body request = {"unama": "Lintang", "uemail": "lintangwisesa@ymail.com", "upassword": "12345"}

    POST /login 
    body request = {"uemail": "lintangwisesa@ymail.com", "upassword": "12345"}

    PUT /update 
    body request = {ufoto ualamat ukabkota utelp uid}
    ```

- __Unastore product__

    ```bash
    GET /product

    GET /product/{ product_id }
    ```

- __Cart__

    ```bash
    GET /cart

    GET /cart/{ user_id }
    
    POST /cart 
    body request = {cpid cuid cjumlah}
    ```

- __File__

    ```bash
    GET /file/{ filename.extension }
    
    POST /file
    ```

- __Unasense__

    ```bash
    GET /iot/{ unafeeder_id }
    
    GET /iotlast/{ unafeeder_id }
    
    POST /iot 
    body request = {iid, isuhuu, isuhua, ilembab, ipressu, ialti, itangki}
    
    GET /xdk/{ unafeeder_id }
    
    GET /xdklast/{ unafeeder_id }
    
    POST /xdk 
    body request = {xid, xsuhu, xdo, xph, xamonia, xtds, xtangki}
    ```

<hr>

__Unafeed for Garuda Hacks__ © 2020
