function [Y, Y_w] = vl_myfc(X, W, dzdy)
%regular fully connected layer

[n1,n2,n3,n4,n5] = size(X);

X_t = reshape(X, n1*n2*n3*n4,n5); %%%10773*30

if nargin < 3
    Y = W * X_t;
else
    Y = W' * dzdy;%%% 10773*30    %%%dzdy 20*30
    Y_w = dzdy*X_t';%%%20*10773
end