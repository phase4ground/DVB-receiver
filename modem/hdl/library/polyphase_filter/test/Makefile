

# VERILOG_SOURCES = 	$(PWD)/../polyphase_filter.v \
# 					$(PWD)/../../multiply_accumulate/multiply_accumulate.v \
# 					$(PWD)/../../multiply_accumulate_behavioural/multiply_accumulate_behavioural.v \
# 					$(PWD)/../../fir_filter/fir_filter.v \
# 					$(XILINX_VERILOG_LIB)/src/glbl.v

# VERILOG_SOURCES = 	$(PWD)/../polyphase_filter.v \
# 					$(PWD)/../../fir_filter/fir_filter.v \
# 					$(PWD)/../../multiply_accumulate_behavioural/multiply_accumulate_behavioural.v

VERILOG_SOURCES = 	$(PWD)/../polyphase_filter_axi-lite.v \
					$(PWD)/../../fir_filter/fir_filter_axi-lite.v \
					$(PWD)/../../multiply_accumulate_behavioural/multiply_accumulate_behavioural.v
					
# COMPILE_ARGS = -s glbl -y $(XILINX_VERILOG_LIB)/src/unisims

TOPLEVEL = polyphase_filter
MODULE = test_polyphase_filter

include $(shell cocotb-config --makefiles)/Makefile.inc
include $(shell cocotb-config --makefiles)/Makefile.sim

wave:
	gtkwave waveform.vcd waveform.gtkw