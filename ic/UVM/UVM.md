[返回主页](../../README.md)

## UVM

&emsp; UVM（Universal Verification Methodology）是基于System Verilog的验证方法学。

&emsp; 基本结构如下：

```systemverilog
class name extends uvm_xxx;

 extern function              new(string name = "name", uvm_component parent);
 extern virtual function void build_phase(uvm_phase phase);
 extern virtual function void connect_phase(uvm_phase phase);
 extern virtual function void end_of_elaboration_phase(uvm_phase phase);
 extern virtual function void start_of_simulation_phase(uvm_phase phase);
 extern virtual function void extract_phase(uvm_phase phase);
 extern virtual function void check_phase(uvm_phase phase);
 extern virtual function void report_phase(uvm_phase phase);
 extern virtual function void final_phase(uvm_phase phase);

 `uvm_component_utils_begin(name)
  uvm_field_int(xxx, UVM_ALL_ON)
 `uvm_component_utils_end

endclass
```

**参考文献**

1 《UVM实战》

[返回主页](../../README.md)

<script type="text/javascript">
  document.body.style.backgroundColor='#fdefe6';
</script>