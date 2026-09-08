```mermaid
graph LR  
 Proveedor(("Proveedor / Usuario"))  
 SIGAF(("SIGAF PL"))  
  
 subgraph Portal de Autogestión de Proveedores  
 CU01["CU-01: Lectura, Precisión y Edición de Valores o Montos de IVA"]  
 CU02["CU-02: Transmisión de Valores o Montos Concretos a SIGAF PL"]  
 end  

 Proveedor --> CU01  
 CU01 --> CU02  
 CU02 --> SIGAF
