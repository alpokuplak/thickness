disp("Perhitungan Thickness Of Brackets")
W	= input ("Masukkan nilai W  = ")
k	= input ("Masukkan nilai k1 = ")
x	= input ("Masukkan nilai tk = ")
mprintf("1 = Iya \n2 = Tidak \n")
a   = input ("Iya atau Tidak Bracket menggunakan Flange? = ")
if a==1 then C =95/100
end
if a==2 then C =12/10   
end
y = input ("masukan nilai tmax =")
mprintf("W = %g  k1 = %g  tk = %g  tmax = %g  C = %g \n",W,k,x,y,C)
W	= W
k	= k
x	= x
C	= C
t 	= C*((W/k)^(-3))+x
y   = y
if ((5+x)>t>y)then
    mprintf ("t = %g \n",t)
else 
    mprintf ("Error")
end
