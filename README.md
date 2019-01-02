# ARQMA-API

### For exmple daemon:

```
daemon := arqma.NewDaemonClient("http://127.0.0.1:19994/json_rpc")
blockCount, err := daemon.GetBlockCount()
if err != nil {
    fmt.Println(err)
     return
} 
fmt.Println("Count:", blockCount)

```

### For exmple wallet:
```
wallet := arqma.NewWalletClient("http://127.0.0.1:19996/json_rpc", "user", "pass")
balance, err := wallet.GetBalance()
if err != nil {
	fmt.Println(err)
	return
}
fmt.Println("balance:", balance)
```
