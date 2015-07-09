roap_ev
====

```rb
# Subscriber
class GameObject
  
  #--subscribe :on_space
  def attack
    puts "ATTACKKKKK"
  end
end
```
```rb
# Publisher
class InputManager
  
  def keydown c
    
    if c == Space
      Roap::Ev::fire :on_space
    end
  end
end
```
