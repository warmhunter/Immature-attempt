# Immature-attempt
创意编程课作业
<html><body><pre>
<span style="color: #E2661A;">int</span> num=100;
Yuan[]&nbsp;yuans=<span style="color: #33997E;">new</span> Yuan[num];
<span style="color: #33997E;">void</span> <span style="color: #006699;"><b>setup</b></span>(){
&nbsp;&nbsp;<span style="color: #006699;">fullScreen</span>();
&nbsp;&nbsp;<span style="color: #006699;">size</span>(600,600);
&nbsp;&nbsp;<span style="color: #669900;">for</span>(<span style="color: #E2661A;">int</span> i=0;i&lt;num;i++)
&nbsp;&nbsp;&nbsp;&nbsp;{yuans[i]=<span style="color: #33997E;">new</span> Yuan(<span style="color: #006699;">random</span>(0,<span style="color: #D94A7A;">width</span>),<span style="color: #006699;">random</span>(0,<span style="color: #D94A7A;">height</span>),<span style="color: #006699;">random</span>(0,20));}
}
<span style="color: #33997E;">void</span> <span style="color: #006699;"><b>draw</b></span>(){
&nbsp;&nbsp;<span style="color: #006699;">background</span>(0);
&nbsp;&nbsp;<span style="color: #669900;">for</span>(<span style="color: #E2661A;">int</span> i=0;i&lt;num;i++)
&nbsp;&nbsp;&nbsp;&nbsp;{yuans[i].update();
&nbsp;&nbsp;&nbsp;&nbsp;yuans[i].display();
&nbsp;&nbsp;
&nbsp;&nbsp;}
}
<span style="color: #33997E;">class</span> Yuan
{<span style="color: #E2661A;">float</span> x,y,r;
&nbsp;&nbsp;Yuan(<span style="color: #E2661A;">float</span> x,<span style="color: #E2661A;">float</span> y,<span style="color: #E2661A;">float</span> r)
&nbsp;&nbsp;{<span style="color: #33997E;">this</span>.x=x;
&nbsp;&nbsp;&nbsp;<span style="color: #33997E;">this</span>.y=y;
&nbsp;&nbsp;&nbsp;<span style="color: #33997E;">this</span>.r=r;}
&nbsp;<span style="color: #33997E;">void</span> update()
&nbsp;{x+=<span style="color: #006699;">random</span>(-1,1);
&nbsp;y+=<span style="color: #006699;">random</span>(-1,1);
&nbsp;r+=<span style="color: #006699;">random</span>(-1,1);}
&nbsp;<span style="color: #33997E;">void</span> display()
&nbsp;{<span style="color: #006699;">fill</span>(<span style="color: #006699;">random</span>(0,59),<span style="color: #006699;">random</span>(0,121),<span style="color: #006699;">random</span>(0,209));
&nbsp;<span style="color: #006699;">noStroke</span>();
&nbsp;<span style="color: #006699;">ellipse</span>(x,y,r,r);}
&nbsp;}

</pre></body></html>
