Gradient Descent : 

Gradient descent is not only used in training linear regression, but also to train the most advanced deep neural network model.
  
-  We can use gradient descent to minimise any function, not just the simple cost function. But also where the number are parameters are upto n

As J(w1, w2, w3, …, wn, b)

- Our objective is minimize J.
 ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcVLJSrs1MxtkfMt7mnRekUBAmV5kaJdltE-7x1fEGYM75cZ0bPA3nKXByqNahhFzKNYvPQ9W-UJlWkhPoo2HmfruZDbKbnkgl-cfKjzRJCxJy88Xrvj420pJ1hPDtgIBfaZh60eyhRBZkHqrYLpDg2P5p3?key=UrYzmsmRHfLYmCQJPTAPJA)
 
For this we have started with some values of w, and b and keep changing the value to w, and b until we reduce J(w, b) to a point where it is minimum.  
  
There are also possibilities when there are more than one minimum point for J(w,b)
 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcZLKMyOeJvLc-mZQW1n2BG7XvvphtQcbfe0Q8j3J2Jgz_6jzMqBE5ezQrr1XW4k-LcWMQmwp_GgNyakD7cCiX-zm0FP4T-1S8tqCtIC1FUN_ePMe4WR3NAC5XldXdH3FdPCeCFD6vWXI2h7jDheFQnomPR?key=UrYzmsmRHfLYmCQJPTAPJA)


Above image is a representation of a neural network model, but it is here just for an example of a neural network.(Example of you wanting to climb down to the valleys the mountain as soon as possible)

Our person shows where the J(w,b) is now, as our goal is to find such values of w, and b such that J(w,b) minimizes to its lowest value, so what gradient descent algorithm does, is finding the most steepest point in 360 degree, and start descending from here, and do this at every step. 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXejptL55w_cZ_KFMVNrwB46Z0TspdI5kesvydSbpaC51kpoxTnWYj6PcvWc58SKUAHvDouRlun9NnAo_d6fGVFw8433bUdek1Wbc2mecFVaNf2SlWyYBLjcuAgXaoJr9NvNzqzFfN4PclOclK4DKZ7aozOZ?key=UrYzmsmRHfLYmCQJPTAPJA)


This algorithm may descend to any of the valley here, depending on the starting point.

These two points here are called local minima.

Mathematical Expressions to implement Gradient Descent.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcvAaLPckaKAKkhDjIkJuztszMirkAdSzMILqnvmqLeAFA9vE64QFU0ox-nktNk7uulKlDZvY4ujvIAq6VX9_ReWpvt6GETPJhjQXtN6PnnBW1WonGk5pREa8Ce5RnrJS5orzKRNjqmDPDvyXnrzljoXnx7?key=UrYzmsmRHfLYmCQJPTAPJA)


At every step value of w is being updated to the R.H.S. value.

This means we are subtracting some little amount from w to change its value
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXed9Xtc5prh06dN8EOoOhhrDwXrOj-6CIpTFFNlvJ2oezgfvABdGhUkXzJf4hf-GxDrZ1sxUZcapxRq6VVpikV2T4Z_VPnFUj7QVbR9cAcYQTmhz9t_4f-s_vw_ehabID7ZcRBvdt6p44zImdQETOykf30?key=UrYzmsmRHfLYmCQJPTAPJA)


Alpha here is the learning rate, it may be any value between 0, and 1.

Alpha controls how bit down you step down the hill.

- Large alpha value -> aggressive gradient descent (taking huge steps)
- Small alpha value -> baby steps


![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd2S0tzbwxZy2R3VjMPgSEyho8zt2Uea4wphKkJE8dTdecOF_lX_xHP-Z1KVOE8433gezfcpSHz129ZqVeeCsSOcCAXmEHwmSWzg9AiJ_TGFnqQK_WpOQsEpjrty5vMZvny8efkwEefdrZYTNEwPrsltwzC?key=UrYzmsmRHfLYmCQJPTAPJA)

For now only understand that this derivative is determining the direction.
As our model now has two parameters so we also have to apply updations to our b parameter.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcyF3eLKnRp05x1qhJSEAzTZy4XsBFF6KVrWkwxdFFgmSwXaWpfPiPq0aUSJmptc-MoNq7MwnkvFw7T1Xf7rBZbRtFf3M9klE1xJ0Q6uMjH01lfsv24BaYwfjNOE4Xe4-qZWo69bZ-OgKgSXNof8Y63Qvo?key=UrYzmsmRHfLYmCQJPTAPJA)


The updates for b look like this, we have to repeat these steps until we reach a point of convergence or local minima(from where w, and b does not change more as you take more steps).

  Note : It is necessary to update both w and b simultaneously.
 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfC8cbJrLyJWrCE8QafWS5OTe6IqDw9MUDp8uhe30Ye4l2dz5cBGOzjExIEdGBof4hFxMHKIWcp1kl-Hae7m9Ikrnxn_6tlVa9GoGSvki3Vu43cgGW4RtueQns5fhN-eOXcrxJsqeielQu7_dbJcUor8ZU?key=UrYzmsmRHfLYmCQJPTAPJA)

### Cause of Why Simultaneous Update is mendatory
Not updating simultaneously affects the function for next term, as the other value gets updated(w for example) then J(w,b) gives a different value as it should because of early updates of actual w.

#### Gradient Descent Intuition : 
Gradient Descent for Linear regression, intuition

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXduv8jrUkKstrQdW1PfZdeiqtjHd2V0QkoOgktprWkoKONFX2ihhx1ILfIefWrvrNN3KHlvM1n08Yt2KiYsR4hB7kJ9exLh4dtI6uZrrvyduNFSEHpUpeaWwsnw__5oaQ87pe_ZY9OngPMzZxXKw04XiD-l?key=UrYzmsmRHfLYmCQJPTAPJA)


When J(w) is greater than the minimum value the slope is positive as shown in figure, slope is 2 which is positive, and alpha(learning rate) is always so we are subtracting a positive value.

Which means we are moving backwards on the graph.
Similarly, 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfqNqrMUtK8TfvxQbLkGxXgm444Kb64dTomP24KPjV_UXgSZyPwlFMMRl6q-vxwoAuITtL_vNvJTkwHEO9tTluk7p4vqQVo9OGOscMzWezlhKfvOIaSMe9CPEkXbCN_t6zQ1bjJGdp98ypDQQ63RRvSF2s?key=UrYzmsmRHfLYmCQJPTAPJA)

When value of J(w) is less than that of minimum point, then slope is negative(-2) so 

W = w - alpha(-number)

W = w + apha(number)

Which means we are adding something positive to w, thus we are increasing its value, so it also go down wards.

##### Learning Rate Alpha : 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfQpVBhqFMJ9ekTZBwSeKt7oJhuxKV84MpvF9m81aNghq-hD0VRElsjPK8P7hPHBNmxHZ8f2CfEUOp2zw9aVo59d8866-fAnWckJgsGVEOLbXj-rGpPhlhNNV3Tn62VrhgSFnCY4n3-Zr5yVAVR6Qi3MmK6?key=UrYzmsmRHfLYmCQJPTAPJA)

If the learning rate is too small as shown in first figure it mean we are taking very small steps toward the minimum value of J(w) similarly if it is too large it takes larger steps, but in this case it may overshoot(go beyond the minimum value which is not good as we never reach our goal the minimum value).

#### Gradient Descent for Linear Regression : 
Fitting straight lines using gradient descent.


![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXchsKqc8TpLGpu3Vrq95A7aO8rzus-Jza9vSdh0ElKMnIltqGVAHyY3ciTkGgtKCL2D9EeDz5l_pomBYW8ccz-i19GxT9UDQTeZDhraQ7PDl6vs9yiQtlshYVAwbjjsGSMc1UpBxOzQZ9qymFAwjPtvIIE?key=UrYzmsmRHfLYmCQJPTAPJA)

Linear regression model formula, and Cost function are familiar, 

On the right down side we have derivatives calculated for the terms.

Why are derivatives like that?

Derivative w.r.t. W : 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdbTnt3sJ-HFquOQ0mh4ViLzhV5p1NZHgBM4PpEBRn86bM8HGhurJGDeUAp34nV8E6YR9Wzip9Dxp2fIKRQga5WaLFvQxsciIZmSGS00JiPJ7biml1Htt30KslMTu5AwnCnv7G96VWQBrVKTgR1LA4SpTNO?key=UrYzmsmRHfLYmCQJPTAPJA)


First we plug in the value for f(x) which is wx +b 
Then we take partial derivate w.r.t. X which gives us that result.
For b we don’t have xi so the equation is simply as follows.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd_zuUJK7lZhN8ou1ECDxpmffmFmV1uUMxCzHdq8iuUhqechEzU9X_e_JfCiN5BzLhRfosl2RD1gh2XVhwEwwQdwVXtfGoztuABkQ1h6HEc2TDnL2c2rsSUYl1JvwkJITAFvEJqokfw5pPvmobVqMz1J2za?key=UrYzmsmRHfLYmCQJPTAPJA)

#### Running Gradient Descent : 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXckK7Xh_LyMcO73ZTw1K1rluzYN4aGk2N8dyy764xee0XZbvALrizGw6IV2D_HP8rygjWIj9chnQkTpiZaE4g-ABPiydVMsc70C9Z3-2yzL9-tpiBdYJu6m1bT6Xzpd52dI7UQ2V_P1vUdNOwI_CmaB8pr-?key=UrYzmsmRHfLYmCQJPTAPJA)

  
We apply gradient descent again and again, until we get the global minima point, above is the representation in the contour plot. The yellow line is the best fit which is found at the center of contour plot.