# chesss.js


https://www.javatpoint.com/ai-alpha-beta-pruning

https://www.hackerearth.com/blog/developers/minimax-algorithm-alpha-beta-pruning/


Psuedocode:

//code

      function minimax(node, depth, maximizingPlayer)
      if depth = 0 or node is a terminal node
         return the utility of the node
     if maximizingPlayer
         bestValue := ??
      for each child of node
         v := minimax(child, depth ? 1, FALSE)
         bestValue := max(bestValue, v)
      return bestValue 
      else (* minimizing player *)
         bestValue := +?
         for each child of node
             v := minimax(child, depth ? 1, TRUE)
             bestValue := min(bestValue, v)
         return bestValue
