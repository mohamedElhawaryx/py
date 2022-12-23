# knowledge representation task
                                              from logic import *
                                              # Q 1.1
                                              # in English : Carrots color is orange
                                              carrots = Symbol("carrots")
                                              orange = Symbol("orange")
                                              knowledge_for_question1 = And(
                                                  Implication(carrots, orange)
                                              )

# Q 1.2
# in English : " if person is vegetarian , person likes carrots "
person = Symbol("person")
vegetarian = Symbol("vegetarian(x)")
like = Symbol("like")
like_person_carrots = Symbol("like(x, carrots)")
knowledge_for_question2 = And(Implication(vegetarian, like_person_carrots))

                                              # Q 1.3
                                              # in English : " student pass if he studies hard "
                                              pass_exam = Symbol("pass(x)")
                                              study_hard = Symbol("study_hard(x)")
                                              knowledge_for_question3 = Implication(study_hard, pass_exam)

# Q 1.4
# in English : " who will pass? "
Pass = Symbol("? pass(who)")
knowledge_for_question4 = And(Pass)

# Q 1.5
# in English : " which course teacher teach ? "
teaches = Symbol("? teaches(course, which)")
knowledge_for_question5 = And(teaches)

                                              # Q 1.6
                                              # in English : " if x & y are enemies, x hate y and x fight y "
                                              x = Symbol("x")
                                              y = Symbol("y")
                                              enemies = Symbol(f"enemies({x}, {y})")
                                              hates = Symbol(f"hates({x}, {y})")
                                              fight = Symbol(f"fight({x}, {y})")
                                              knowledge_for_question6 = And(Implication(enemies, And(hates, fight)))
                                              
                                              
                                              
                                              
                                              
                                              
                                              
                                              
                                              
                                from logic import *

# Q 2.1
#  read(maria, logic programming book) ==> by(peter lucas)
maria = Symbol("maria")
peter_lucas = Symbol("peter lucas")
read = Symbol(f" read ({maria}, logic programming book)")
by = Symbol(f"by ({peter_lucas})")
knowledge_for_question1 = And(Implication(read, by))


                                                            # Q 2.2
                                                            # is_girl(x) ==> like(x, shopping)
                                                            is_girl = Symbol("is_girl(x)")
                                                            shopping = Symbol("shopping")
                                                            like = Symbol(f"like(x, {shopping} )")
                                                            knowledge_for_question2 = And(Implication(is_girl, like))

# Q 2.3
# ? likes( x , shopping)
who = Symbol("?")
knowledge_for_question3  = And(who ,like)

                                                            # Q 2.4
                                                            # city( x ,big , crowdy) ==> hates(kirke, x)
                                                            city = Symbol("city(x, big, crowdy)")
                                                            hates = Symbol("kirke, x")
                                                            knowledge_for_question4 = And(Implication(city, hates))


