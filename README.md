# Punto-Q.5.81
Further Analysis
XY= linspace(-pi,pi,100);

>> YX =XY;
>> [X,Y] = meshgrid(XY,YX);

>> Z = sin(2.*Y).*cos(2.*X).*exp(-sqrt(X.^2+Y.^2)./2);

>> subplot (2,1,1);

>> mesh (X,Y,Z)

>> xlabel (‘X’),ylabel(‘Y’),zlabel(‘Z’)

>> title (‘Mesh Plot’)

>> subplot(2,1,2);

>> surf (X,Y,Z)

>> xlabel(‘X’),ylabel(‘Y’),zlabel(‘Z’)

>> title(‘Surf Plot’)
