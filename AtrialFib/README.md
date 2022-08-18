## **Atrial Fibrillation**
Atrial fibrillation (AFib) is a condition where the heartbeat becomes erratic and the upper chambers of 
the heart quiver and shake. If there’s a lurking blood clot, this shaking can break it loose and send it up
through the blood vessels to the brain, where it can cause a stroke. People with AFib have a 5 times greater
likelihood of having a stroke, and doctors typically put patients with the condition on blood-thinning medications 
that prevent clots
 

#### **Sinus rhythm**
In a normal heart rhythm, the sinus node generates the impulse that causes the atria to contract.
This impulse is propagated to the AV node and then throughout ventricles, causing the ventricles to contract.
This process results in a very regular rhythm called **sinus rhythm**.

##### Atrial Fibrillation
In Atrial Fibrillation, instead of the SA node being the sole location that begins the depolarization of the atria,
there are multiple locations around the atria that will spontaneously and haphazardly generate an impulse.
Each of these impulses causes a partial contraction of the atria, but no single impulse depolarizes the entire atria,
so there is no coherent contraction of the atria. Occasionally, one of these impulses will reach the AV node, 
which will then cause a ventricular contraction. 

But this occurs at random times, so ventricular contractions occur irregularly.

When can we examine features of the ECG signal to detect atrial fibrillation? First, 
there is no P-wave because there is no coherent depolarization of the atria to cause an electrical disturbance
large enough to create the P-wave. 
 - Instead, we see a fibrillating wave in the T-Q segment.
 - Second, the QRS complexes are very irregular.
 
Atrial fibrillation is associated with an increased risk of stroke. 
Because the atria are not contracting completely, stagnant pools of blood will form in the atria. 
These pools can form blood clots that are then circulated through the bloodstream. 
As these clots pass through progressively smaller and smaller arteries, they may eventually obstruct blood 
flow to the brain and cause a stroke.

Now we have seen how atrial fibrillation occurs physiologically and why it’s a potentially dangerous condition.
Next, we will build an algorithm that automatically detects atrial fibrillation and other arrhythmias from the ECG signal.