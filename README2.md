

# ref url 

https://studygolang.com/articles/11448


# must be set
```
&tls.Config{  
    PreferServerCipherSuites: true,  
    // 仅仅使用拥有汇编实现的Curve  
    CurvePreferences: []tls.CurveID{  
        tls.CurveP256,  
        tls.X25519, // Go 1.8 only  
    },  
} 


tls.TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384,  
tls.TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384,  
tls.TLS_ECDHE_ECDSA_WITH_CHACHA20_POLY1305, // Go 1.8 only  
tls.TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305,   // Go 1.8 only  
tls.TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256,  
tls.TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256,  

AES-GCM,Chacha20-Poly2305,P256)

srv := &http.Server{  
    ReadTimeout:  5 * time.Second,  
    WriteTimeout: 10 * time.Second,  
    IdleTimeout:  120 * time.Second,  
    TLSConfig:    tlsConfig,  
    Handler:      serveMux,  
}  
log.Println(srv.ListenAndServeTLS("", ""))  

Server.TLSNextProto
[]string{"h2","http/1.1"}

net.ListenTCP keepalive


```
