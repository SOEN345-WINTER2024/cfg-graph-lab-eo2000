## Eden Oliel 40211989 

## Lab 7 :
Part 1 - Basic Calculator : 
1) Draw the CFG graph for onClick()<img width="1161" alt="Screenshot 2024-03-08 at 3 58 59 PM" src="https://github.com/SOEN345-WINTER2024/cfg-graph-lab-eo2000/assets/116772744/b6b0dc30-4eff-4f4a-afd2-de99e48ed5c2">

2)  Compute node coverage for this CFG
- TR : [1][2][3][4][5][6][7][8][9][10][11][12][13][14][15][16][17][18][19][20][21][22]
- Test paths : [1,2,22][1,3,22][1,4,22][1,5,22][1,6,22][1,7,22][1,8,22][1,9,22][1,10,22][1,11,22][1,12,22][1,13,22][1,14,22][1,15,22][1,16,22][1,17,18,22][1,17,19,22][1,17,20,22][1,17,21,22]

3) Compute edge coverage for this CFG
- TR : [1,2][1,3][1,4][1,5][1,6][1,7][1,8][1,9][1,10][1,11][1,12][1,13][1,14][1,15][1,16][1,17][17,18][17,19][17,20][17,21][18,22][19,22][20,22][21,22]
[2,22][3,22][4,22][5,22][6,22][7,22][8,22][9,22][10,22][11,22][12,22][13,22][14,22][15,22][16,22]
- Test paths : [1,2,22][1,3,22][1,4,22][1,5,22][1,6,22][1,7,22][1,8,22][1,9,22][1,10,22][1,11,22][1,12,22][1,13,22][1,14,22][1,15,22][1,16,22][1,17,18,22][1,17,19,22][1,17,20,22][1,17,21,22]

4) Compute edge-pair coverage for this CFG
- TR : [1,2,22],[1,2,22],[1,3,22],[1,4,22],[1,5,22],[1,6,22],[1,7,22],[1,8,22],[1,9,22],[1,10,22],[1,11,22],,[1,12,22],[1,13,22],[1,14,22],[1,15,22],[1,16,22],[1,17,18],[1,17,19], [1,17,20],[1,17,21],[17,18,22],[17,19,22],[17,2022],[17,21,22]
- Test paths : [1,2,22][1,3,22][1,4,22][1,5,22][1,6,22][1,7,22][1,8,22][1,9,22][1,10,22][1,11,22][1,12,22][1,13,22][1,14,22][1,15,22][1,16,22][1,17,18,22][1,17,19,22][1,17,20,22][1,17,21,22]

5) Draw the EFG graph for the Calculator App
   ![IMG_3417](https://github.com/SOEN345-WINTER2024/cfg-graph-lab-eo2000/assets/116772744/c312c31e-5de3-4ad0-9897-2920376c0760)


Part 2 - Project App : 
1) Draw the CFG graph for onCreate()
   
 @Override
    protected void onCreate(@Nullable Bundle savedInstanceState) {
        // Restore the Saved State first so that it is available to
        // OnContextAvailableListener instances
        mSavedStateRegistryController.performRestore(savedInstanceState);
        mContextAwareHelper.dispatchOnContextAvailable(this);
        super.onCreate(savedInstanceState);
        ReportFragment.injectIfNeededIn(this);
        if (mContentLayoutId != 0) {
            setContentView(mContentLayoutId);
        }
    }

<img width="433" alt="Screenshot 2024-03-15 at 3 29 36 PM" src="https://github.com/SOEN345-WINTER2024/cfg-graph-lab-eo2000/assets/116772744/c0d64f93-7a09-449f-bf5f-8c67432a03f1">


2) Compute node coverage for this CFG
  - TR : [1], [2], [3], [4], [5], [6]
  - Test paths : [1,2,3,4,5,6]
4) Compute edge coverage for this CFG
  - TR : [1,2], [2,3], [3,4], [4,5], [5,6]
  - Test paths : [1,2,3,4,5,6]

5) Compute edge-pair coverage for this CFG
  - TR :
  - Test paths :
6) Draw the EFG graph: 
