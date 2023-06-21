# Apple-and-Orange-hackeranck-solution-Javasctipt

function countApplesAndOranges(s, t, a, b, apples, oranges) {
    // Apple and Orange (hackeRrank): (javascript)
    let forApple = apples.map(apple => a + apple)
    let forOrange = oranges.map(orange => b + orange)
    let countApple = 0; let countOrange = 0;
     
    for(let i in forApple){
      if(forApple[i] >= s && forApple[i] <= t){
        countApple++
      }
    }
    for(let i in forOrange){
      if(forOrange[i] >= s && forOrange[i] <= t){
        countOrange++
      }
    }

    console.log(countApple)
    console.log(countOrange)
}

countApplesAndOranges(7, 10, 4, 12, [2,3,-4], [3,-2,-4])
