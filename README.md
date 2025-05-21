# Ex5-Animator-Movement

## Aim :

To develop a animator movement for a player using unity.

## Algorithm :

## Step 1 : 

Import necessary models.

## Step 2 : 

 Right-click -> Create -> Animator Controller.

## Step 3 : 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4 : 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5 : 

Drag Animator Controller to the GameObject in the Inspector.

## Program :

### DEVELOPED BY : VINODINI R
### REG NO : 212223040244

## PlayerController:


```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called before the first frame update
    void Start()
    {
        animator = this.gameObject.GetComponent <Animator>();
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        animator.SetFloat("InputX", InputX);
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputY", InputY);
    }
}


```
## Output :

![image](https://github.com/user-attachments/assets/90c60bd8-06b3-4dc2-87e9-1a157d51c6be)
![image](https://github.com/user-attachments/assets/ff82992b-0ab6-4987-b5d6-36bb712d8994)
![image](https://github.com/user-attachments/assets/8c58fbed-f2e0-4fa4-a54f-9cd2188bc54f)


## Result :

Thus, An animator movement for a player using unity is developed successfully.
