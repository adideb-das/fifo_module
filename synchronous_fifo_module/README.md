
# Synchronous FIFO Module in Verilog
FIFO module is a module used for the purpose of synchronization and handshakes between modules.
 
DEPTH of FIFO: number of slots/rows in FIFO 

WIDTH of FIFO: number of bits that can be stored in each slot/rows

As the name suggests, data read and data write use the same clock frequency.

It has the following input-output ports:-

wr_en, wr_data, full, empty, rd_en, rd_data , wr_ptr, rd_ptr

# FIFO write operation

FIFO can store/write wr_data at every posedge of the clock based on wr_en till it`s full . The write pointer gets incremented on every data write in FIFO memory.

# FIFO read operation

Like the write operation , the read operation can be read from the FIFO module at every posedge of the clock based on the rd_en till it`s empty. The read pointer gets incremented on every data read from FIFO memory. 