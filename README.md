# laravel9_get_client_ip_address
## Example 1:
```Dockerfile
$clientIP = request()->ip();    
dd($clientIP);
```
## Example 2:
```Dockerfile
<?php
  
namespace App\Http\Controllers;
  
use Illuminate\Http\Request;
  
class UserController extends Controller
{
    /**
     * Display a listing of the resource.
     *
     * @return \Illuminate\Http\Response
     */
    public function index(Request $request)
    {
    	$clientIP = $request->ip();   
        dd($clientIP);
    }
}
```
## Example 3:
```Dockerfile
$clientIP = \Request::ip();
dd($clientIP);
```
## Example 4:
```Dockerfile
$clientIP = \Request::getClientIp(true);
dd($clientIP);
```
