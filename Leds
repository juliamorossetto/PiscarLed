module leds(
    input CLOCK_50,
    input [3:0]KEY,
    output [0:0]LEDG
);
   
reg [32:0] contador = 0;
reg registrador = 0;

assign LEDG[0] = ~registrador;
   
always@(posedge KEY[0])
    begin
        if(contador >= 5)
            begin
                registrador <= ~registrador;
                contador <= 0;
            end
        //--   
        else
            begin
                contador = contador + 1;
            end
        end 
endmodule
