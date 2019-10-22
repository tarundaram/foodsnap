do {
      . 
      . PRODUCE ITEM
      .
      wait(empty);
      wait(mutex);
      .  
      . PUT ITEM IN BUFFER
      .
      signal(mutex);
      signal(full);

} while(1);  
