<!DOCTYPE html>
<html>
<body>

<canvas id="canvas" width="500" height="500" style="border:1px solid #d3d3d3;">
Your browser does not support the HTML canvas tag.</canvas>

<script type="text/javascript">
            // request first frame
			
    requestAnimationFrame(update);
    const canvas = document.getElementById("canvas");
	const ctx = canvas.getContext('2d');
	



            // constructor
            function rect(id, x, y, width, height, fill, stroke, strokewidth) {
                this.x = x;
                this.y = y;
                this.id = id;
                this.width = width;
                this.height = height;
                this.fill = fill || "gray";
                this.stroke = stroke || "skyblue";
                this.strokewidth = strokewidth || 2;
                //this.redraw(this.x, this.y);
                return (this);

            return rect;
        }
		
		
		    // constructor
            function player(id, lvl, stamina, xp, stats1, stats2, stats3, name) {
                this.id = id;
                this.lvl = lvl || 1;
                this.stamina = stamina;
                this.xp = xp || 10000;
                this.stats1 = stats1 || 4;
                this.stats2 = stats2 || 3;
                this.stats3 = stats3 || 4;
                this.name = name || 'john';
                
                return (this);

            return player;
        }
	
    // We dont need any vector functionality as the operations are so 
    // simple we can just use undefined object.
    const A = {x : 0, y : 0};
    const B = {x : 0, y : 0};    
    const circleCenter = {x : 100, y : 100};
    const halfLineLen = 125;
    var time = 0;
    const mouse = { x : 100, y : 100 }
    const r = 45;
    const speed = 0.01;
	var score = 0;
    
    addEventListener("mousemove",(e)=>{
        mouse.x =  (e.clientX - canvas.width / 2.0) - 5.0;
        mouse.y = -(e.clientY - canvas.height / 2.0) + 5.0;
    })
    

    // Function to check intercept of line seg and circle
    // A,B end points of line segment
    // C center of circle
    // radius of circle
    // returns true if touching or crossing else false   
    function doesLineInterceptCircle(A, B, C, radius) {
        var dist;
        const v1x = B.x - A.x;
        const v1y = B.y - A.y;
        const v2x = C.x - A.x;
        const v2y = C.y - A.y;
        // get the unit distance along the line of the closest point to
        // circle center
        const u = (v2x * v1x + v2y * v1y) / (v1y * v1y + v1x * v1x);
        
        
        // if the point is on the line segment get the distance squared
        // from that point to the circle center
        if(u >= 0 && u <= 1){
            dist  = (A.x + v1x * u - C.x) ** 2 + (A.y + v1y * u - C.y) ** 2;
        } else {
            // if closest point not on the line segment
            // use the unit distance to determine which end is closest
            // and get dist square to circle
            dist = u < 0 ?
                  (A.x - C.x) ** 2 + (A.y - C.y) ** 2 :
                  (B.x - C.x) ** 2 + (B.y - C.y) ** 2;
        }
        return dist < radius * radius;
     }
  
  
    function update() {     
		//console.log(mouse.x);
		//console.log(mouse.y);
		canvas.width = window.innerWidth/2;
		canvas.height = window.innerHeight/2;
		//canvas.width = 414px;
		//canvas.height = 896px;
		//console.log(score);
		
         ctx.clearRect(0, 0, canvas.width, canvas.height);
         time += speed;
         A.x = - Math.cos(time) * halfLineLen;
         A.y = - Math.sin(time) * halfLineLen;
         B.x =  Math.cos(time) * halfLineLen;
         B.y =  Math.sin(time) * halfLineLen;


         circleCenter.x = mouse.x;
         circleCenter.y = mouse.y;
          
         
         const intersects = doesLineInterceptCircle(A, B, circleCenter, r);

        ctx.setTransform(1, 0, 0, -1, canvas.width / 2, canvas.height / 2);

        ctx.lineWidth = 2.0;
        ctx.fillStyle = intersects ? "green" : "red";
		if(intersects){
			score++
		}
     
        ctx.beginPath();
        ctx.arc(circleCenter.x, circleCenter.y, r, 0, Math.PI * 2);	
        ctx.fill();

        ctx.strokeStyle = "rgba(150,50,50,0.8)";
        ctx.lineWidth = 6;         

        ctx.beginPath();  // You dont need to use moveTo after beginPath
        ctx.lineTo(A.x, A.y);  
        ctx.lineTo(B.x, B.y);
        ctx.stroke();

        ctx.setTransform(1,0,0,1,0,0);
		
		
		ctx.strokeStyle = "black";
		ctx.font = "900 50px sans-serif";
		canvas.textAlign = "start";
		ctx.fillStyle = "#ff0000";
		ctx.fillText(score, canvas.width / 2, 50);
		
		pc.xp = score;
        requestAnimationFrame(update);
    }
		var rects = [];
	    rects.push(new rect("Red-Rectangle", 15, 35, 65, 60, "red", "black", 10));
        rects.push(new rect("Green-Rectangle", 60, 80, 70, 50, "green", "black", 10));
        rects.push(new rect("Blue-Rectangle", 125, 25, 25, 25, "blue", "black", 10));
		
		var pc = new player(11, 1, 100, 1000, 3, 4, 4, 'john')
	update();
    </script>

</body>
</html>

