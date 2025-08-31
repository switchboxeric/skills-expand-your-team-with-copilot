# Example Issue Template Usage

This document shows an example of how the issue templates work when filled out by a teacher.

## Example: Add New Activity Request

Here's what a completed "Add New Activity" template would look like:

---

**Title:** [NEW ACTIVITY] Add Drama Club

**Activity Name:** Drama Club

**Activity Description:** Students will learn acting, directing, and stage production. They will participate in script reading, character development exercises, and perform in seasonal school plays. This club helps develop public speaking skills, creativity, and teamwork.

**Meeting Days:** Monday, Wednesday

**Meeting Time:** 3:30 PM - 5:30 PM

**Maximum Participants:** 18

**Supervising Teacher:** Ms. Rodriguez

**Activity Category:** Arts

**Special Requirements or Notes:** 
- Requires access to the school auditorium
- Need budget for props and costumes
- Parent permission forms required for evening performances

**Acceptance Criteria:** ✅ All boxes checked
- Add the new activity to the activities database with all provided details
- Activity should appear in the main activities list on the website  
- Activity should be filterable by day, time, and category
- Teachers should be able to register/unregister students for this activity
- Activity should respect the maximum participant limit

---

## What Copilot Gets From This

With this structured information, Copilot can immediately understand:

1. **Exact implementation needed:** Add "Drama Club" to the database
2. **Database format required:**
   ```python
   "Drama Club": {
       "description": "Students will learn acting, directing, and stage production...",
       "schedule": "Monday, Wednesday, 3:30 PM - 5:30 PM", 
       "schedule_details": {
           "days": ["Monday", "Wednesday"],
           "start_time": "15:30",
           "end_time": "17:30"
       },
       "max_participants": 18,
       "participants": []
   }
   ```
3. **Files to modify:** `src/backend/database.py`
4. **Testing needed:** Verify it appears on website and filters work
5. **Category classification:** Should be classified as "arts" activity type

## Benefits Demonstrated

### For the Teacher (Ms. Rodriguez):
- ✅ No need to understand database formats or file structures
- ✅ Guided through all necessary information  
- ✅ Clear examples helped her format times and descriptions
- ✅ Confidence that all required details were provided

### For Copilot:
- ✅ Zero ambiguity about what needs to be implemented
- ✅ Exact technical specifications provided
- ✅ Clear acceptance criteria for testing
- ✅ Complete context for making implementation decisions

This is exactly the kind of clear, structured request that allows Copilot to implement changes efficiently without needing additional clarification from teachers.